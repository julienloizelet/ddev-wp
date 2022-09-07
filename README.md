# DDEV stack for WordPress

The purpose of this repo is to share my WordPress [DDEV](https://ddev.readthedocs.io/en/stable/) stack.


<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**

- [Quick start](#quick-start)
  - [DDEV installation](#ddev-installation)
  - [Prepare DDEV WordPress environment](#prepare-ddev-wordpress-environment)
  - [WordPress installation](#wordpress-installation)
- [Usage](#usage)
  - [Test your own plugin](#test-your-own-plugin)
- [License](#license)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Quick start

_We will suppose that you want to test on a WordPress 5.6.5 instance. Change the version number if you prefer another
release._

### DDEV installation

This project is fully compatible with DDEV 1.21.1, and it is recommended to use this specific version.
For the DDEV installation, please follow the [official instructions](https://ddev.readthedocs.io/en/stable/#installation).
On a Linux distribution, you can run:
```
sudo apt-get -qq update
sudo apt-get -qq -y install libnss3-tools
curl -LO https://raw.githubusercontent.com/drud/ddev/master/scripts/install_ddev.sh
bash install_ddev.sh v1.21.1
rm install_ddev.sh
```


### Prepare DDEV WordPress environment

The final structure of the project will look like below.

```
wp-sources
│   
│ (WordPress sources)    
│
└───.ddev
│   │   
│   │ (Cloned sources of this repo)
│   
└───my-own-modules (only if you want to test some of your module(s))
    │   
    │
    └───yourVendorName-yourModuleName
       │   
       │ (Sources of a module)
         
```

- Create an empty folder that will contain all necessary sources:
```
mkdir wp-sources
```
- Create an empty `.ddev` folder for DDEV and clone our pre-configured DDEV repo:

```bash
mkdir wp-sources/.ddev && cd wp-sources/.ddev && git clone git@github.com:julienloizelet/ddev-wp.git ./
```
- Copy some configurations file:

```bash
cp .ddev/config_overrides/config.wp565.yaml .ddev/config.wp565.yaml
```
- Launch DDEV

```bash
cd .ddev && ddev start
```
This should take some times on the first launch as this will download all necessary docker images.


### WordPress installation

```bash
cd wp-sources
wget https://wordpress.org/wordpress-5.6.5.tar.gz
tar -xf wordpress-5.6.5.tar.gz wordpress
cp -r wordpress/. ./
rm -rf wordpress
rm wordpress-5.6.5.tar.gz
ddev start
ddev exec wp core install --url='https://wp565.ddev.site' --title='WordPress' --admin_user='admin' 
--admin_password='admin123' --admin_email='admin@admin.com'

```


## Usage

### Test your own plugin

```bash
cd wp-sources
mkdir -p my-own-modules/your-module && cd my-own-modules/your-module
git clone git@github.com:your-git-repo/your-module-repo.git ./
```

## License

[MIT](LICENSE)
