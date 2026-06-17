---
name: enso-org__enso__claude
source: https://github.com/enso-org/enso/blob/4135f929f1046ee4ab62d9d09c155377e8542a1f/build_tools/build/CLAUDE.md
repo: enso-org/enso
kind: claude-md
stars: 7438
last_pushed: 2026-06-13T04:51:14Z
license: apache-2.0
score: 8
domains: [cli-tools, systems-programming, build-systems]
tags: [rust, architecture, build-pipeline]
curated: 2026-06-16
curated_by: config-scout
---

# enso-org/enso — claude-md

**Why it's worth keeping:** The 'Module map' provides essential mental models for directory navigation, while the 'Patterns' section offers concrete technical constraints that prevent common errors like blocking I/O in async contexts.

**Summary:** Provides a detailed architectural map of the build toolchain, including module responsibilities and critical dependency constraints.

**Source credibility:** Highly credible; part of a large-scale (7k+ stars), actively maintained open-source project.

**Recency:** 

**Source:** [enso-org/enso/build_tools/build/CLAUDE.md](https://github.com/enso-org/enso/blob/4135f929f1046ee4ab62d9d09c155377e8542a1f/build_tools/build/CLAUDE.md) · 7438★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# enso-build

Domain logic of the Enso build CLI. Owns the Target concept (see `README.md` in
`build_tools/`) and implements all the artifact producers.

**Status: legacy**, slated for replacement by Bazel. Maintain existing targets,
but don't add new ones when a Bazel target can cover the same case.

## Module map

Each module handles one artifact family or one integration:

- `engine/` + `engine.rs` — Scala/Java engine (runtime + language server).
  Shells out to SBT. Note: the Scala Project Manager is no longer part of this
  bundle — the Electron app uses the TypeScript `app/project-manager-shim/`
  instead.
- `ide/` + `ide.rs` — Top-level IDE target. Glues GUI and backend.
- `project/` + `project.rs` — GUI side: invokes pnpm/Vite.
- `release/` + `release.rs` — Cutting releases, signing, uploading assets.
- `repo/` + `repo.rs` — Git repo state, commit hashes, branch conventions.
- `changelog/` + `changelog.rs` — Parses + validates `CHANGELOG.md` entries
  (one-per-PR rule).
- `rust/` — Rust workspace helpers (running cargo across members, WASM builds).
- `ci/`, `ci_gen/`, `ci.rs`, `ci_gen.rs` — CI-matrix and GitHub Actions YAML
  generation inputs. Output is written by `enso-bu
```

</details>
