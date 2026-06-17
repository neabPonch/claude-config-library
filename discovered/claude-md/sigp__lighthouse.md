---
name: sigp__lighthouse
source: https://github.com/sigp/lighthouse/blob/176cce585c1ba979a6210ed79b6b6528596cdb8c/CLAUDE.md
repo: sigp/lighthouse
kind: claude-md
stars: 3448
last_pushed: 2026-06-14T03:54:33Z
license: apache-2.0
score: 9
domains: [systems-programming, blockchain, rust]
tags: [rust, high-performance, consensus]
curated: 2026-06-15
curated_by: config-scout
---

# sigp/lighthouse — claude-md

**Why it's worth keeping:** It includes highly specific 'anti-patterns' (e.g., Rayon usage, panic prevention) that are critical for systems programming, which provides much more value than just basic CLI commands. The structure—commands, architecture, quality standards, and technical patterns—serves as an elite template for any complex repository.

**Summary:** Provides exhaustive build/test instructions alongside a high-level architectural map and strict coding standards.

**Source credibility:** Extremely high; Lighthouse is a foundational Ethereum consensus client with massive community adoption.

**Recency:** Very current, showing active maintenance and modern Rust development practices.

**Source:** [sigp/lighthouse/CLAUDE.md](https://github.com/sigp/lighthouse/blob/176cce585c1ba979a6210ed79b6b6528596cdb8c/CLAUDE.md) · 3448★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

**Important**: Always branch from `unstable` and target `unstable` when creating pull requests.

### Building and Installation

- `make install` - Build and install the main Lighthouse binary in release mode
- `make install-lcli` - Build and install the `lcli` utility binary
- `cargo build --release` - Standard Rust release build
- `cargo build --bin lighthouse --features "gnosis,slasher-lmdb"` - Build with specific features

### Testing

- `make test` - Run the full test suite in release mode (excludes EF tests, beacon_chain, slasher, network, http_api)
- `make test-release` - Run tests using nextest (faster parallel test runner)
- `make test-beacon-chain` - Run beacon chain tests for all supported forks
- `make test-slasher` - Run slasher tests with all database backend combinations
- `make test-ef` - Download and run Ethereum Foundation test vectors
- `make test-full` - Complete test suite including linting, EF tests, and execution engine tests
- `cargo nextest run -p <package_name>` - Run tests for a specific package
- `cargo nextest run
```

</details>
