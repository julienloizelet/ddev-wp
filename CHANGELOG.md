# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/)
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [2.5.4](https://github.com/julienloizelet/ddev-wp/releases/tag/v2.5.4) - 2023-02-15
[Compare with previous release](https://github.com/julienloizelet/ddev-wp/compare/v2.5.3...v2.5.4)
### Changed
- Release workflow test

---


## [2.5.3](https://github.com/julienloizelet/ddev-wp/releases/tag/v2.5.3) - 2023-02-15
[Compare with previous release](https://github.com/julienloizelet/ddev-wp/compare/v2.5.2...v2.5.3)
### Changed
- Release workflow test

---

## [2.5.2](https://github.com/julienloizelet/ddev-wp/releases/tag/v2.5.2) - 2023-02-15
[Compare with previous release](https://github.com/julienloizelet/ddev-wp/compare/v2.5.1...v2.5.2)
### Fixed
- Revert CI Release GitHub action previous fix

---

## [2.5.1](https://github.com/julienloizelet/ddev-wp/releases/tag/v2.5.1) - 2023-02-15
[Compare with previous release](https://github.com/julienloizelet/ddev-wp/compare/v2.5.0...v2.5.1)
### Fixed
- Change CI Release GitHub action

---

## [2.5.0](https://github.com/julienloizelet/ddev-wp/releases/tag/v2.5.0) - 2023-02-15
[Compare with previous release](https://github.com/julienloizelet/ddev-wp/compare/v2.4.0...v2.5.0)
### Changed
- Configure `crowdsec` container to log in file
 
### Added
- Add `redis-commander` service yaml
- Add `crowdsec-without-plugin` service yaml
- Add a custom `cache-actions-from-plugin-folder.php` script for CrowdSec WordPress plugin test


## [2.4.0](https://github.com/julienloizelet/ddev-wp/releases/tag/v2.4.0) - 2023-01-31
[Compare with previous release](https://github.com/julienloizelet/ddev-wp/compare/v2.3.0...v2.4.0)
### Changed
- Exclude some php files for CrowdSec auto prepend directive in Nginx configuration

### Added
- Add a custom `cache-actions.php` script for CrowdSec WordPress plugin test


## [2.3.0](https://github.com/julienloizelet/ddev-wp/releases/tag/v2.3.0) - 2023-01-31
[Compare with previous release](https://github.com/julienloizelet/ddev-wp/compare/v2.2.0...v2.3.0)
### Changed
- Change DDEV compatibility by using `1.21.4` ddev version

## [2.2.0](https://github.com/julienloizelet/ddev-wp/releases/tag/v2.2.0) - 2022-09-07
[Compare with previous release](https://github.com/julienloizelet/ddev-wp/compare/v2.1.0...v2.2.0)
### Changed
- Change DDEV compatibility by using `1.21.1` ddev version
- Change `crowdsec` bouncer plugin path

### Added
- Add `DDEV_EXPECTED_VERSION.txt` file with post-start hook to compare current and expected DDEV version
- Add `portainer` service docker-compose file
---
## [2.1.0](https://github.com/julienloizelet/ddev-wp/releases/tag/v2.1.0) - 2022-07-15
[Compare with previous release](https://github.com/julienloizelet/ddev-wp/compare/v2.0.0...v2.1.0)
### Changed
- Change DDEV compatibility by using `1.19.3` ddev version

### Added
- Add `maxmind-download` command
---
## [2.0.0](https://github.com/julienloizelet/ddev-wp/releases/tag/v2.0.0) - 2022-03-31
[Compare with previous release](https://github.com/julienloizelet/ddev-wp/compare/v1.4.1...v2.0.0)
### Changed
- Change DDEV compatibility by using `1.19.1` ddev version
- Change `find-ip` command for ddev 1.19.1 compatibility

### Added
- Add `nginx-config` host command to reload nginx configuration with a custom configuration file
- Add `phpinfo` script
---
## [1.4.1](https://github.com/julienloizelet/ddev-wp/releases/tag/v1.4.1) - 2022-03-04
[Compare with previous release](https://github.com/julienloizelet/ddev-wp/compare/v1.4.0...v1.4.1)
### Added
- Added installation test for more WordPress and PHP versions 
---
## [1.4.0](https://github.com/julienloizelet/ddev-wp/releases/tag/v1.4.0) - 2022-03-04
[Compare with previous release](https://github.com/julienloizelet/ddev-wp/compare/v1.3.0...v1.4.0)
### Added
- Config for WordPress 5.0, 5.0.1, 5.2, and 5.9
---
## [1.3.0](https://github.com/julienloizelet/ddev-wp/releases/tag/v1.3.0) - 2021-12-02
[Compare with previous release](https://github.com/julienloizelet/ddev-wp/compare/v1.2.0...v1.3.0)
### Added
- Config for WordPress 4.9,5.3,5.4,5.5,5.6,5.7 and 5.8
---
## [1.2.0](https://github.com/julienloizelet/ddev-wp/releases/tag/v1.2.0) - 2021-11-18
[Compare with previous release](https://github.com/julienloizelet/ddev-wp/compare/v1.1.0...v1.2.0)
### Added
- Config for WordPress 5.7.4
---
## [1.1.0](https://github.com/julienloizelet/ddev-wp/releases/tag/v1.1.0) - 2021-11-05
[Compare with previous release](https://github.com/julienloizelet/ddev-wp/compare/v1.0.0...v1.1.0)
### Added
- Commands and config for crowdsec
- Playwright container for end-to-end tests

### Fixed
- Fix the `create-watcher` command for the second parameter
---
## [1.0.0](https://github.com/julienloizelet/ddev-wp/releases/tag/v1.0.0) - 2021-10-15

### Added
- Initial release
