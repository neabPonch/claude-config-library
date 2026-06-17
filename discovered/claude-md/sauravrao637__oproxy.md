---
name: sauravrao637__oproxy
source: https://github.com/sauravrao637/oproxy/blob/3396d88e6e5e879e58e43d5271a403b8514bdbd6/CLAUDE.md
repo: sauravrao637/oproxy
kind: claude-md
stars: 439
last_pushed: 2026-06-14T21:22:49Z
license: mit
score: 9
domains: [backend, networking, rust]
tags: [architecture-heavy, system-design, middleware]
curated: 2026-06-15
curated_by: config-scout
---

# sauravrao637/oproxy — claude-md

**Why it's worth keeping:** Uses high-density information like flowcharts for the request lifecycle and tables for internal side-channels to prevent AI logic errors; includes critical edge cases like binary body handling.

**Summary:** Provides deep architectural context including request lifecycles, middleware insertion orders, and state management.

**Source credibility:** Highly credible; a well-starred open-source project with very recent maintenance.

**Recency:** Current, providing specific guidance for modern Rust and Node/Yarn workflows.

**Source:** [sauravrao637/oproxy/CLAUDE.md](https://github.com/sauravrao637/oproxy/blob/3396d88e6e5e879e58e43d5271a403b8514bdbd6/CLAUDE.md) · 439★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
# Build
cargo build
cargo build --release

# Build the React UI assets required by Rust include_str! routes
corepack enable
yarn --cwd src/design install --frozen-lockfile
yarn --cwd src/design build

# Run all Rust tests with release warning policy
RUSTFLAGS="-D warnings" cargo test

# Run a single test by name
cargo test <test_name>

# Run tests in a specific module
cargo test middleware::plugins::jwt_inspector

# Lint
cargo clippy -- -D warnings

# Run the proxy. A clean checkout will build src/design/dist automatically
# if Node/Yarn are available; explicit UI build is still faster in CI.
cargo run
```

> **Critical:** run the full test suite before release, not only `cargo test --lib`. Browser tests live under `tests/browser` and use Playwright.

## Architecture

### Three-layer separation

1. **Transport** (`main.rs`, `core/engine.rs`) — hyper accept loop, CONNECT handling, MITM TLS, reqwest forwarding  
2. **Traffic manipulation** (`middleware/`) — inspect, rewrite, throttle, pause, mock  
3. **Control plane** (`management.rs`, `api/`, `st
```

</details>
