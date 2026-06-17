---
name: surrealdb__surrealdb
source: https://github.com/surrealdb/surrealdb/blob/3dab345f8ea7ca02178200d53d1f777560202bea/CLAUDE.md
repo: surrealdb/surrealdb
kind: claude-md
stars: 32390
last_pushed: 2026-06-10T18:24:15Z
license: other
score: 9
domains: [database, rust, wasm, backend]
tags: [rust, testing-protocol, bug-investigation, custom-dsl]
curated: 2026-06-15
curated_by: config-scout
---

# surrealdb/surrealdb — claude-md

**Why it's worth keeping:** The 'Bug Investigation Protocol' offers an actionable chain-of-thought for debugging, while the detailed '.surql' test specification enables the AI to write complex language tests accurately.

**Summary:** Provides deep technical context including specific Rust patterns, WASM compatibility constraints, and a custom test file format.

**Source credibility:** High; SurrealDB is a widely used, highly-starred database project with active maintenance.

**Recency:** Current; includes modern ecosystem references like MCP and specific Rust/WASM patterns.

**Source:** [surrealdb/surrealdb/CLAUDE.md](https://github.com/surrealdb/surrealdb/blob/3dab345f8ea7ca02178200d53d1f777560202bea/CLAUDE.md) · 32390★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides essential context for AI assistants working with the SurrealDB codebase.

## Project Overview

SurrealDB is a multi-model database built in Rust supporting document, graph, relational, time-series, geospatial, and key-value data models. It can run embedded, in browser (WASM), at the edge, or as a distributed cluster.

## Project Structure

```
surrealdb/           # Main SDK crate
surrealdb/core/      # Core database engine (query execution, storage)
surrealdb/mcp/       # Model Context Protocol server (stdio + HTTP)
surrealdb/server/    # HTTP, WebSocket, gRPC server
surrealdb/types/     # Public types and derive macros
surrealism/          # Surrealism (WASM plugin system) crates
language-tests/      # SurrealQL test suite (.surql files)
tests/               # Integration tests (CLI, HTTP, WebSocket, GraphQL)
```

## Common Commands

```bash
# Build and run dev server
cargo run --no-default-features --features storage-mem,http,scripting -- start --log trace --user root --pass root memory

# Format code (REQUIRED before commits)
cargo make fmt

# Run clippy lints
cargo make ci-clippy

# Run all tests
cargo test

# Run language tests
cd language-test
```

</details>
