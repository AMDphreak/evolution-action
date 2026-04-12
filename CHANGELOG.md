# Changelog

## [2.1.1] - 2026-04-10

### Changed

- **Pinning defaults:** `engine-version` default `v1.3.2`; `rules-repo` default `AMDphreak/evolution-rules-code`; `rules-version` remains `v1.0.0`. Aligns with repositories as hosted on GitHub today.
- **`extensions` default** matches the engine (includes `.js`, `.ts`, `.astro`).
- Documentation leads with fully pinned examples; link:COMPATIBILITY.md[COMPATIBILITY.md] records the action ↔ engine ↔ rules matrix.

## [2.1.0] - 2026-04-10

### Added

- **Floating `latest` tag** so workflows can use `uses: AMDphreak/equivalence-engine-action@latest`; documentation recommends pinning semver or SHA for reproducible CI.

### Changed

- Documentation and defaults renamed from Evolution Engine to **Equivalence Engine**; repository defaults now use `AMDphreak/equivalence-engine`, checkout paths `equivalence-engine-tool` / `equivalence-rules-dir`, and binary `equivalence-engine`.

## [2026-03-21] - Initial Release

- Initial release of the GitHub Action.
- Wraps `qt-upgrader` CLI.
