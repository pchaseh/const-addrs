# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

### Categories each change fall into

* **Added**: for new features.
* **Changed**: for changes in existing functionality.
* **Deprecated**: for soon-to-be removed features.
* **Removed**: for now removed features.
* **Fixed**: for any bug fixes.
* **Security**: in case of vulnerabilities.


## [Unreleased]
### Added
- Initial support for `ipnet` network types

### Changed
- Rename the "ipnet" feature to "ipnetwork" to match the dependency.
- Rename the "mac" feature to "macaddr" to match the dependency.


## [0.2.0] - 2025-05-11
This release is identical to `0.1.2`. This is re-released as `0.2.0` since the changes
were semver breaking.


## [0.1.2] - 2025-05-10
### Added
- Use `const`-compatible constructors in `ipnetwork`, allowing using the macros in const
  contexts.

### Changed
- Disable default features on `ipnetwork` dependency. Strips out `serde` as a
  transitive dependency.
- Upgrade `ipnetwork` dependency from `0.20` to `0.21`. This is a breaking change
  since the `ipnetwork` dependency is part of the public API of this library.
