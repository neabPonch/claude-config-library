---
name: cube-js__cube__claude
source: https://github.com/cube-js/cube/blob/87ae095c69588a77d2711968a66e07c9764c2e6b/rust/cubestore/CLAUDE.md
repo: cube-js/cube
kind: claude-md
stars: 20179
last_pushed: 2026-06-16T04:02:38Z
license: other
score: 9
domains: [distributed-systems, rust, data-infrastructure]
tags: [rust, olap, storage-engine]
curated: 2026-06-16
curated_by: config-scout
---

# cube-js/cube — claude-md

**Why it's worth keeping:** The 'Important Notes' section proactively addresses risks like custom library forks and specific nightly requirements, while the DI documentation clarifies service instantiation patterns.

**Summary:** Provides deep architectural context for a Rust-based distributed OLAP engine, including detailed crate breakdowns and module hierarchies.

**Source credibility:** High; Cube is a major open-source project with 17k+ stars and active maintenance.

**Recency:** Current; references very recent Rust nightly toolchains from 2025.

**Source:** [cube-js/cube/rust/cubestore/CLAUDE.md](https://github.com/cube-js/cube/blob/87ae095c69588a77d2711968a66e07c9764c2e6b/rust/cubestore/CLAUDE.md) · 20179★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

CubeStore is the Rust-based distributed OLAP storage engine for Cube.js, designed to store and serve pre-aggregations at scale. It's part of the larger Cube.js monorepo and serves as the materialized cache store for rollup tables.

## Architecture Overview

### Core Components

The codebase is organized as a Rust workspace with multiple crates:

- **`cubestore`**: Main CubeStore implementation with distributed storage, query execution, and API interfaces
- **`cubestore-sql-tests`**: SQL compatibility test suite and benchmarks
- **`cubehll`**: HyperLogLog implementation for approximate distinct counting
- **`cubedatasketches`**: DataSketches integration for advanced approximate algorithms
- **`cubezetasketch`**: Theta Sketch implementation for set operations
- **`cuberpc`**: RPC layer for distributed communication
- **`cuberockstore`**: RocksDB wrapper and storage abstraction

### Key Modules in `cubestore/src/`

- **`metastore/`**: Metadata management, table schemas, partitioning, and distributed coordination
- **`queryplanner/`**: Query plann
```

</details>
