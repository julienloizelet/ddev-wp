# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).


## [2.2.0] - 2022-09-07

### Changed
- Change DDEV compatibility by using `1.21.1` ddev version
- Change `crowdsec` bouncer plugin path

### Added
- Add `DDEV_EXPECTED_VERSION.txt` file with post-hook to compare current and expected DDEV version
- Add `portainer` service docker compose file

## [2.1.0] - 2022-07-15

### Changed
- Change DDEV compatibility by using `1.19.3` ddev version

### Added
- Add `maxmind-download` command

## [2.0.0] - 2022-03-31

### Changed
- Change DDEV compatibility by using `1.19.1` ddev version
- Change `find-ip` command for ddev 1.19.1 compatibility

### Added
- Add `nginx-config` host command to reload nginx configuration with a custom configuration file
- Add `phpinfo` script

## [1.4.1] - 2022-03-04

### Added
- Added installation test for more WordPress and PHP versions 

## [1.4.0] - 2022-03-04

### Added
- Config for WordPress 5.0, 5.0.1, 5.2, and 5.9

## [1.3.0] - 2021-12-02

### Added
- Config for WordPress 4.9,5.3,5.4,5.5,5.6,5.7 and 5.8

## [1.2.0] - 2021-11-18

### Added
- Config for WordPress 5.7.4

## [1.1.0] - 2021-11-05

### Added
- Commands and config for crowdsec
- Playwright container for end-to-end tests

### Fixed
- Fix the `create-watcher` command for the second parameter

## [1.0.0] - 2021-10-15

### Added
- Initial release
