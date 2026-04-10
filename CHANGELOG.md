# Changelog

## [2.1.0] - 2026-04-10

### Added

- **Floating `latest` tag** on this repository so workflows can use `uses: AMDphreak/equivalence-engine-action@latest`; documentation recommends pinning semver or SHA for reproducible CI.

### Changed

- Documentation and defaults renamed from Evolution Engine to **Equivalence Engine**; repository defaults now use `AMDphreak/equivalence-engine`, `AMDphreak/equivalence-rules-code`, checkout paths `equivalence-engine-tool` / `equivalence-rules-dir`, and binary `equivalence-engine`.

## [2026-03-21] - Initial Release

- Initial release of the GitHub Action.
- Wraps `qt-upgrader` CLI.
