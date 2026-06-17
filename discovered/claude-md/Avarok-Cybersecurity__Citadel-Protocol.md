---
name: Avarok-Cybersecurity__Citadel-Protocol
source: https://github.com/Avarok-Cybersecurity/Citadel-Protocol/blob/dedbf5c6765d4d0221f240f1470d7f9619e61bcd/CLAUDE.md
repo: Avarok-Cybersecurity/Citadel-Protocol
kind: claude-md
stars: 162
last_pushed: 2026-06-14T16:24:13Z
license: apache-2.0
score: 9
domains: [rust, security, networking, cryptography]
tags: [rust-workspace, architecture-guide, security-protocol, build-commands]
curated: 2026-06-15
curated_by: config-scout
---

# Avarok-Cybersecurity/Citadel-Protocol — claude-md

**Why it's worth keeping:** Includes high-value 'Common Development Patterns' code snippets and explains the impact of feature flags on threading models, which helps the LLM avoid architectural errors.

**Summary:** Comprehensive guide covering detailed Cargo commands, complex multi-crate workspace architecture, and specific security protocols.

**Source credibility:** High; highly specialized cryptographic protocol with a structured, mature Rust workspace structure.

**Recency:** Very current; utilizes modern Rust tooling like cargo-make and nextest.

**Source:** [Avarok-Cybersecurity/Citadel-Protocol/CLAUDE.md](https://github.com/Avarok-Cybersecurity/Citadel-Protocol/blob/dedbf5c6765d4d0221f240f1470d7f9619e61bcd/CLAUDE.md) · 162★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

### Building
```bash
# Build all packages
cargo build --all

# Build with specific features
cargo build --features sql,redis

# Build release version
cargo build --release
```

### Testing
```bash
# Run local tests (without external backends)
cargo make test-local

# Run comprehensive tests (requires SQL/Redis setup)
# Set environment variables first:
export TESTING_SQL_SERVER_ADDR_CLIENT="mysql://root:password@localhost/hyxewave2,postgres://nologik:password@localhost/hyxewave2,sqlite:/home/runner/hyxewave2.db,redis://127.0.0.1:6379/2"
export TESTING_SQL_SERVER_ADDR_SERVER="mysql://root:password@localhost/hyxewave,postgres://nologik:password@localhost/hyxewave,sqlite:/home/runner/hyxewave.db,redis://127.0.0.1:6379/1"
cargo make test

# Run specific package tests
cargo nextest run --package citadel_sdk --features=localhost-testing

# Run multi-threaded tests
cargo nextest run --package citadel_sdk --features=multi-threaded,localhost-testing

# Run a single test
cargo nextest run test_name_here
```

### Linting and Formatting
```bash
# Format code
cargo ma
```

</details>
