---
name: mxsm__rocketmq-rust
source: https://github.com/mxsm/rocketmq-rust/blob/cce620c1f3d44f60f0d114630e5a052bce85b457/CLAUDE.md
repo: mxsm/rocketmq-rust
kind: claude-md
stars: 1485
last_pushed: 2026-06-15T01:16:53Z
license: apache-2.0
score: 9
domains: [rust, distributed-systems, backend]
tags: [rust, cargo-workspace, monorepo, testing-automation]
curated: 2026-06-15
curated_by: config-scout
---

# mxsm/rocketmq-rust — claude-md

**Why it's worth keeping:** Features highly specific 'targeted testing' commands to prevent tool execution bloat in large repos and defines a strict 'definition of done' through exact Clippy/Fmt flags.

**Summary:** Provides a detailed architectural map of a complex multi-crate Rust workspace, including distinct instructions for standalone sub-projects.

**Source credibility:** High; the project is a major distributed systems implementation with high star count and very recent maintenance.

**Recency:** Current; uses modern Rust toolchain standards and structure compatible with contemporary AI agent workflows.

**Source:** [mxsm/rocketmq-rust/CLAUDE.md](https://github.com/mxsm/rocketmq-rust/blob/cce620c1f3d44f60f0d114630e5a052bce85b457/CLAUDE.md) · 1485★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# RocketMQ Rust - Claude Code Instructions

This is an unofficial Rust implementation of Apache RocketMQ, a distributed messaging and streaming platform.

## Project Overview

- **Language**: Rust (nightly toolchain, MSRV 1.85.0)
- **Architecture**: Multi-crate Cargo workspace with standalone projects
- **Key Components**: Broker, NameServer, Client, Store, Remoting, Controller, Proxy
- **License**: Apache-2.0 OR MIT

## Repository Structure

### Main Workspace
Root Cargo workspace containing core crates:
- `rocketmq-broker` - Message broker implementation
- `rocketmq-client` - Client SDK
- `rocketmq-common` - Shared utilities and types
- `rocketmq-store` - Storage engine
- `rocketmq-remoting` - Network communication layer
- `rocketmq-namesrv` - Name server for routing
- `rocketmq-controller` - Cluster controller
- `rocketmq-proxy` - Proxy layer
- `rocketmq-auth` - Authentication module
- `rocketmq-filter` - Message filtering
- `rocketmq-runtime` - Async runtime abstractions
- `rocketmq-macros` - Procedural macros
- `rocketmq-error` - Error types
- `rocketmq-tools/*` - Admin CLI, TUI, and store inspection tools
- `rocketmq-dashboard/rocketmq-dashboard-common` - Dashboard shared cod
```

</details>
