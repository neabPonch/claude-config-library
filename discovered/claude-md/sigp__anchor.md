---
name: sigp__anchor
source: https://github.com/sigp/anchor/blob/e65ec5ed9673010088a56dfb6cfc222641f0b729/CLAUDE.md
repo: sigp/anchor
kind: claude-md
stars: 67
last_pushed: 2026-06-12T00:18:45Z
license: apache-2.0
score: 9
domains: [rust, blockchain, systems-programming]
tags: [rust-workspace, system-architecture, command-reference]
curated: 2026-06-15
curated_by: config-scout
---

# sigp/anchor — claude-md

**Why it's worth keeping:** It includes 'system mental models' like event flow and dependency direction, which helps an LLM reason about side effects in complex multi-crate workspaces.

**Summary:** Provides a highly detailed breakdown of project commands alongside a deep architectural map of the system's thread model and component interactions.

**Source credibility:** High; maintained by Sigma Prime, a reputable organization in the Ethereum/SSV ecosystem.

**Recency:** Current; specifically references Claude Code and modern Rust development patterns.

**Source:** [sigp/anchor/CLAUDE.md](https://github.com/sigp/anchor/blob/e65ec5ed9673010088a56dfb6cfc222641f0b729/CLAUDE.md) · 67★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## About Anchor

Anchor is an open-source implementation of the Secret Shared Validator (SSV) protocol, written in Rust and maintained by Sigma Prime. It serves as a validator client for Ethereum's proof-of-stake consensus mechanism using secret sharing techniques.

## Common Commands

### Build and Install

```bash
# Build the project in release mode
cargo build --release

# Install Anchor to your path
make install

# Build for specific architectures
make build-x86_64      # Build for x86_64 Linux (requires cross)
make build-aarch64     # Build for aarch64 Linux (requires cross)

# Create release tarballs
make build-release-tarballs
```

### Testing

```bash
# Run all tests in release mode (standard)
make test
# or
cargo test --release --features "$(TEST_FEATURES)"

# Run all tests in debug mode
make test-debug
# or
cargo test --workspace --features "$(TEST_FEATURES)"

# Run tests with nextest (faster)
make nextest-release
make nextest-debug

# Test a specific crate
cd anchor/common/qbft
cargo test

# Check benchmark code (without running benchmarks)
make check-benc
```

</details>
