---
name: cloudwego__volo
source: https://github.com/cloudwego/volo/blob/92740bad9bfa08ac4af8a6098af9255569af6ab4/CLAUDE.md
repo: cloudwego/volo
kind: claude-md
stars: 2600
last_pushed: 2026-05-19T13:39:27Z
license: apache-2.0
score: 9
domains: [rust, backend, infrastructure]
tags: [workspace-management, dependency-graph, rust]
curated: 2026-06-16
curated_by: config-scout
---

# cloudwego/volo — claude-md

**Why it's worth keeping:** The inclusion of a dependency graph, explicit release order, and a feature flag summary provides the essential 'mental model' needed to manage large scale refactors and publishing workflows.

**Summary:** Provides deep architectural context, crate relationships, and feature flag mappings for a complex multi-crate Rust workspace.

**Source credibility:** High; maintained by CloudWeGo (ByteDance) with significant community adoption.

**Recency:** Current; includes modern Rust 2024 edition context and recent maintenance.

**Source:** [cloudwego/volo/CLAUDE.md](https://github.com/cloudwego/volo/blob/92740bad9bfa08ac4af8a6098af9255569af6ab4/CLAUDE.md) · 2600★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Volo Workspace

For detailed per-crate documentation, see the CLAUDE.md in each sub-crate directory.

## Project Overview

[Volo](https://github.com/cloudwego/volo) is a high-performance Rust RPC framework by CloudWeGo (ByteDance). It supports Thrift, gRPC, and HTTP protocols with fully async design (Tokio), zero-copy optimizations, and middleware via Service/Layer abstractions (motore).

- Rust Edition: 2024
- MSRV: 1.85.0
- Current Version: 0.12.x

## Workspace Structure

```
volo/
├── volo/                   # Core library
├── volo-build/             # Code generation from IDL (Thrift/Protobuf)
├── volo-cli/               # CLI tool (project scaffolding)
├── volo-grpc/              # gRPC implementation
├── volo-http/              # HTTP implementation
├── volo-macros/            # Procedural macros (reserved)
├── volo-thrift/            # Thrift implementation
├── examples/               # Example code
├── benchmark/              # Performance benchmarks
└── tests/code-generation/  # Code generation tests
```

## Crate Dependency Graph

```
                     volo-macros (reserved)
                          |
                          v
    +------------------
```

</details>
