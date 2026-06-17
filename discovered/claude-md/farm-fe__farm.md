---
name: farm-fe__farm
source: https://github.com/farm-fe/farm/blob/2000ef8a790a1b565d1687cfe70564270a826e15/CLAUDE.md
repo: farm-fe/farm
kind: claude-md
stars: 5578
last_pushed: 2026-06-14T13:57:04Z
license: mit
score: 9
domains: [cli-tools, build-systems]
tags: [monorepo, rust, typescript, napi-rs]
curated: 2026-06-16
curated_by: config-scout
---

# farm-fe/farm — claude-md

**Why it's worth keeping:** The architecture section explains the data flow across language boundaries (napi-rs), which is crucial for multi-language debugging; it also includes specific environment variables for specialized testing workflows like insta snapshots.

**Summary:** Provides a deep structural map of a complex Rust/TypeScript bridge and detailed command protocols.

**Source credibility:** Highly credible, coming from a high-star (5.5k+) active build tool repository.

**Recency:** Very current, referencing modern tooling standards like pnpm v9 and Rust 2021 edition.

**Source:** [farm-fe/farm/CLAUDE.md](https://github.com/farm-fe/farm/blob/2000ef8a790a1b565d1687cfe70564270a826e15/CLAUDE.md) · 5578★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Farm is an extremely fast, Vite-compatible web build tool written in Rust (v2.x beta). It is a hybrid Rust + TypeScript monorepo using pnpm workspaces and Cargo workspace. The Rust compiler is exposed to Node.js via napi-rs.

## Key Commands

| Command | Purpose |
|---------|---------|
| `pnpm bootstrap` | First-time setup: install deps + build core packages |
| `pnpm run ready` | Full CI gate (install, clean, build, lint, type-check, test, e2e) |
| `pnpm run test` | TypeScript unit tests (vitest) |
| `pnpm run test-e2e` | E2E tests (vitest + Playwright) |
| `cargo test` | Rust unit tests |
| `cargo test -p farmfe_compiler` | Run tests for a specific Rust crate |
| `cargo test --profile ci-test` | Run Rust tests with CI-optimized profile |
| `pnpm run check` | Biome lint + format |
| `cargo clippy` | Rust linter |
| `cargo check --all --all-targets` | Type-check all Rust code without building |
| `pnpm run spell-check` | cspell across all files |

### Rust snapshot testing uses insta
- `INSTA_UPDATE=always cargo test` to update snapshots
- Or set
```

</details>
