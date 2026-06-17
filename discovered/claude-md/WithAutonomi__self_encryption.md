---
name: WithAutonomi__self_encryption
source: https://github.com/WithAutonomi/self_encryption/blob/0deb040084f94bea2ebb53bda20fa23464bbcfe0/CLAUDE.md
repo: WithAutonomi/self_encryption
kind: claude-md
stars: 138
last_pushed: 2026-06-01T16:04:38Z
license: other
score: 9
domains: [security, cli-tools, rust, cryptography]
tags: [architecture-map, technical-debt-aware]
curated: 2026-06-14
curated_by: config-scout
---

# WithAutonomi/self_encryption — claude-md

**Why it's worth keeping:** The 'Implementation Notes' section explicitly documents critical edge cases (like chunk 0/1 circular dependency handling) and technical debt, preventing the LLM from introducing regressions in the streaming implementation.

**Summary:** Provides comprehensive development commands and deep architectural context for a Rust-to-Python encryption library.

**Source credibility:** High; the repo has substantial stars (138) and very recent activity suggesting a well-maintained tool.

**Recency:** Current; it explicitly mentions Claude Code and utilizes modern development workflows like maturin and cargo-llvm-cov.

**Source:** [WithAutonomi/self_encryption/CLAUDE.md](https://github.com/WithAutonomi/self_encryption/blob/0deb040084f94bea2ebb53bda20fa23464bbcfe0/CLAUDE.md) · 138★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Building and Testing

```bash
# Format code (MANDATORY before commits)
cargo fmt --all

# Run clippy linter with strict settings
cargo clippy --all-features -- -D warnings

# Run all Rust tests
cargo test --release

# Run comprehensive test script (includes Python tests)
./scripts/test.sh

# Build Python package with maturin
maturin develop --features python

# Run Python tests
pytest tests/ -v

# Run benchmarks
cargo bench

# Check for unused dependencies
cargo udeps --all-targets

# Publish dry run
cargo publish --dry-run
```

### Single Test Execution

```bash
# Run a specific Rust test
cargo test test_name --release

# Run a specific Python test
pytest tests/test_file.py::test_name -v

# Run tests with output
cargo test -- --nocapture
```

## Architecture Overview

### Core Encryption Process

The self_encryption crate implements convergent encryption with obfuscation through a three-stage process:

1. **Content Chunking**: Files are split into chunks (up to 1MB each)
2. **Per-Chunk Processing**:
   - Compression (Brotli with configur
```

</details>
