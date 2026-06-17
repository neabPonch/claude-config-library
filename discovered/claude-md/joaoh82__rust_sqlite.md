---
name: joaoh82__rust_sqlite
source: https://github.com/joaoh82/rust_sqlite/blob/f52f04a5ee2e6e61dd4dd2f425baef6b16e7cbd0/CLAUDE.md
repo: joaoh82/rust_sqlite
kind: claude-md
stars: 1076
last_pushed: 2026-06-14T21:58:26Z
license: mit
score: 10
domains: [systems-programming, database-engine, rust, cli-tools]
tags: [mono-repo, architecture-deep-dive, build-optimization]
curated: 2026-06-15
curated_by: config-scout
---

# joaoh82/rust_sqlite — claude-md

**Why it's worth keeping:** It includes specific cargo `--exclude` flags to navigate a complex mono-repo, explains the 'why' behind architectural decisions, and distinguishes between stable context and daily notes.

**Summary:** An elite-tier instruction file that combines high-level architecture, complex workspace build commands, and deep technical constraints.

**Source credibility:** High; 1k+ stars on a specialized systems programming project with recent activity.

**Recency:** Highly current, referencing modern stacks like Tauri 2 and Svelte 5.

**Source:** [joaoh82/rust_sqlite/CLAUDE.md](https://github.com/joaoh82/rust_sqlite/blob/f52f04a5ee2e6e61dd4dd2f425baef6b16e7cbd0/CLAUDE.md) · 1076★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

SQLRite is a from-scratch SQLite-style embedded database written in Rust. It's published on crates.io as `sqlrite-engine` (imported as `use sqlrite::…` — the lib target keeps the short name) and ships as: a REPL binary (`sqlrite`), a Tauri 2 + Svelte 5 desktop app, a Model Context Protocol stdio server (`sqlrite-mcp`), a C FFI shim (`sqlrite-ffi`), and language SDKs (Python via PyO3, Node via napi-rs, Go via cgo, WASM via wasm-bindgen). Phases 1–7 are shipped; the current branch `phase-8-plan` drafts inverted-index + BM25 full-text search and hybrid retrieval.

## Workspace layout

`Cargo.toml` is a workspace whose members are: `.` (the engine, package `sqlrite-engine`, lib `sqlrite`), `desktop/src-tauri`, `sqlrite-ffi`, `sqlrite-ask`, `sqlrite-mcp`, `sdk/python`, `sdk/nodejs`, `benchmarks`. `sdk/wasm` and `sdk/go` are deliberately **not** workspace members (wasm32 target / cgo separation).

- `src/` — engine. Public API is `Connection`/`Statement`/`Rows`/`Row`/`Value` from [src/connection.rs](src/connection.rs), re-exported via [src/lib.rs](src/lib.rs).
```

</details>
