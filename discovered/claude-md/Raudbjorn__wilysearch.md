---
name: Raudbjorn__wilysearch
source: https://github.com/Raudbjorn/wilysearch/blob/cc494a7145792f69b3bc85ae73e1c8c66a941a70/CLAUDE.md
repo: Raudbjorn/wilysearch
kind: claude-md
stars: 0
last_pushed: 2026-05-29T21:44:53Z
license: unknown
score: 9
domains: [rust, search-engine, systems-programming]
tags: [architecture-mapping, dependency-constraints, type-system]
curated: 2026-06-15
curated_by: config-scout
---

# Raudbjorn/wilysearch — claude-md

**Why it's worth keeping:** It identifies specific 'bridge' logic requirements and highlights high-stakes dependency version constraints that would cause build failures if ignored by the AI.

**Summary:** This file documents a complex two-layer type system that bridges a public API to an internal core. It provides critical instructions on how to maintain consistency when adding new fields across these layers.

**Source credibility:** While the repo has low visibility, the documentation exhibits a high level of technical maturity and structural awareness.

**Recency:** Very current; mentions Rust 2024 edition and specific modern dependency conflicts.

**Source:** [Raudbjorn/wilysearch/CLAUDE.md](https://github.com/Raudbjorn/wilysearch/blob/cc494a7145792f69b3bc85ae73e1c8c66a941a70/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

wilysearch is an embedded, HTTP-less Meilisearch engine for Rust. It wraps the milli indexing engine (LMDB-backed) directly, providing full-text search without running a server. All operations are synchronous -- no task queue, no HTTP layer. Rust edition 2024.

## Build & Test Commands

```bash
cargo build                          # build (first build is slow due to milli)
cargo test                           # run all 42 integration tests
cargo test --test index_tests        # run a single test file
cargo test test_basic_search         # run a single test by name
cargo test -- --nocapture            # run tests with stdout visible
cargo check                          # fast type-check without linking
cargo run --example basic_search     # run an example
```

Feature flags:
```bash
cargo build --features surrealdb     # enable SurrealDB vector store backend
```

## Architecture: Two-Layer Type System

The critical design decision to understand: there are **two parallel type systems** that `engine.rs` bridges.

### Public API (what consumers use)
- `s
```

</details>
