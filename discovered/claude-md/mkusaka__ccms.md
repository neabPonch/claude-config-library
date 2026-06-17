---
name: mkusaka__ccms
source: https://github.com/mkusaka/ccms/blob/78517231d5b5b20351d3635f1046dc9f9568f5f3/CLAUDE.md
repo: mkusaka/ccms
kind: claude-md
stars: 3
last_pushed: 2026-06-15T05:53:46Z
license: mit
score: 9
domains: [cli-tools, rust, systems-programming]
tags: [rust, tui, architecture, high-performance]
curated: 2026-06-15
curated_by: config-scout
---

# mkusaka/ccms — claude-md

**Why it's worth keeping:** The 'Common Modifications' section provides highly transferable, step-by-step workflows for adding features without breaking architectural integrity. The 'Architecture Overview' maps the file structure to high-level design patterns, which helps an agent understand logical flow rather than just file locations.

**Summary:** A comprehensive guide that combines exhaustive command sets with a deep architectural breakdown of the system's design patterns (MVU/Clean Architecture). It includes explicit procedural 'recipes' for common code modifications.

**Source credibility:** High; a well-maintained Rust repository with professional documentation standards.

**Recency:** Current; reflects modern Rust development and optimized CLI tool practices.

**Source:** [mkusaka/ccms/CLAUDE.md](https://github.com/mkusaka/ccms/blob/78517231d5b5b20351d3635f1046dc9f9568f5f3/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build Commands

```bash
# Standard release build (optimized)
cargo build --release

# Development build (faster compilation, debugging enabled)
cargo build

# Build with profiling support
cargo build --release --features profiling

# Build with async support
cargo build --release --features async

# Build with all features
cargo build --release --all-features
```

## Test Commands

```bash
# Run all tests
cargo test

# Run tests with output
cargo test -- --nocapture

# Run specific test
cargo test test_name

# Run tests for a specific module
cargo test query::

# Run with verbose output
cargo test -- --test-threads=1 --nocapture
```

## Benchmarking

```bash
# Run all benchmarks
cargo bench

# Run specific benchmark
cargo bench search_benchmark

# Component benchmarks
cargo bench component_benchmark

# Async benchmarks (requires async feature)
cargo bench async_benchmark
```

## Development Commands

```bash
# Check code without building
cargo check

# Format code
cargo fmt

# Lint code
cargo clippy -- -D warnings

# Update dependencies
cargo update

# Generate do
```

</details>
