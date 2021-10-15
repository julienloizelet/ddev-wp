# DDEV-Local stack for WordPress

The purpose of this repo is to share my WordPress [DDEV-Local](https://ddev.readthedocs.io/en/stable/) stack.


<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**

- [Quick start](#quick-start)
  - [DDEV-Local installation](#ddev-local-installation)
  - [Prepare DDEV Magento 2 environment](#prepare-ddev-magento-2-environment)
  - [WordPress installation](#wordpress-installation)
- [Usage](#usage)
  - [Test your own module](#test-your-own-module)
- [License](#license)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## Quick start

_We will suppose that you want to test on a WordPress 5.6.5 instance. Change the version number if you prefer another
release._

### DDEV-Local installation

Please follow the [official instructions](https://ddev.readthedocs.io/en/stable/#installation). On a Linux
distribution, this should be as simple as

    sudo apt-get install linuxbrew-wrapper
    brew tap drud/ddev && brew install ddev


### Prepare DDEV Magento 2 environment

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

```
mkdir wp-sources/.ddev && cd wp-sources/.ddev && git clone git@github.com:julienloizelet/ddev-wp.git ./
```
- Copy some configurations file:

```
cp .ddev/config_overrides/config.wp565.yaml .ddev/config.wp565.yaml
```
- Launch DDEV

```
cd .ddev && ddev start
```
This should take some times on the first launch as this will download all necessary docker images.


### WordPress installation



## Usage

### Test your own module

## License

[MIT](LICENSE)
