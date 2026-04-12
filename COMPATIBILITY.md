# Action ↔ engine ↔ rules compatibility

Pin **three** things in workflows for reproducible CI:

| Pin | Example | Role |
|-----|---------|------|
| This action | `AMDphreak/equivalence-engine-action@v2.1.1` | Composite steps, inputs, checkout paths |
| Engine | `engine-version: v1.3.2` | CLI and `dub` build of `equivalence-engine` |
| Rules | `rules-version: v1.0.0` (and `rules-repo`) | SDL ruleset revision |

## Maintained combinations

| Action tag | Default `engine-version` in `action.yml` | Default `rules-repo` / `rules-version` |
|------------|-------------------------------------------|----------------------------------------|
| `v2.1.1` | `v1.3.2` | `AMDphreak/evolution-rules-code` / `v1.0.0` |

When you release a new **action** version, bump defaults here and extend this table. When the engine CLI breaks compatibility, ship a new **action** minor/major and document the required engine tag.

Floating refs (`@latest`, branch names) are fine for experiments; **do not** rely on them for production pipelines.
