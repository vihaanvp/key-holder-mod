# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.1] - 2026-11-03

### Changed
- **Updated to Minecraft 26.3** (Fabric API 0.161.0+26.3)
- Updated Fabric Loader to 0.19.5
- Updated Fabric Loom to 1.18.2
- Updated Gradle wrapper to 9.7.1
- Updated Cloth Config to 26.3.159
- Updated Mod Menu to 21.0.0
- Bumped mod version to 1.0.1

### Fixed
- Fixed `ClientCommandRegistrationCallback` API for Minecraft 26.3
  - Changed lambda parameter from `registryAccess` to `commandBuildContext` to match new `CommandBuildContext` type

### Maintained
- **26.2 compatibility preserved** in separate `fabric-26.2` build module
  - Uses Fabric Loader 0.18.4 and Fabric API 0.154.0+26.2
  - Separate `mc262_loader_version` property in gradle.properties

### Build
- Both `fabric-26.2` and `fabric-26.3` modules compile and build successfully
- JARs output to respective `build/libs/` directories

## [1.0.0] - 2026-XX-XX

### Added
- Initial release for Minecraft 26.2
- `/keyholder` command with subcommands: `set`, `on`, `off`, `toggle`, `status`
- Configurable key binding via Mod Menu + Cloth Config
- Toggle key binding (unbound by default)
- Config persisted to `config/keyholder.json`

---

[1.0.1]: https://github.com/vihaanvp/key-holder-mod/releases/tag/v1.0.1
[1.0.0]: https://github.com/vihaanvp/key-holder-mod/releases/tag/v1.0.0