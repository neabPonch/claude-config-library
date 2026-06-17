---
name: modular__modular__claude
source: https://github.com/modular/modular/blob/c9aebe6b32e63539eff6366392501e2724af6070/max/kernels/CLAUDE.md
repo: modular/modular
kind: claude-md
stars: 26341
last_pushed: 2026-06-14T09:11:29Z
license: other
score: 9
domains: [systems-programming, ml-infrastructure, performance-engineering]
tags: [mojo, bazel, gpu, benchmarking]
curated: 2026-06-15
curated_by: config-scout
---

# modular/modular — claude-md

**Why it's worth keeping:** Includes critical 'gotcha' warnings like how to avoid shadowed kernel imports during development and detecting GPU thermal throttling. These specific nuances prevent an AI from following incorrect or stale workflows.

**Summary:** Comprehensive guide for building, testing, and benchmarking high-performance Mojo kernels using Bazel. It includes vital instructions for managing development environments and hardware-specific configurations.

**Source credibility:** Highly credible; Modular is a major industry player with high star counts and active maintenance.

**Recency:** Very current, including references to modern hardware like B200 GPUs.

**Source:** [modular/modular/max/kernels/CLAUDE.md](https://github.com/modular/modular/blob/c9aebe6b32e63539eff6366392501e2724af6070/max/kernels/CLAUDE.md) · 26341★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with
code in this repository.

## Repository Overview

This is the MAX Kernels directory containing high-performance compute kernels
written in Mojo. These kernels serve as building blocks for numerical, machine
learning, and other performance-critical workloads. The repository is part of
Modular AI's larger codebase and uses Bazel as its build system.

## Build System

This project uses Bazel for building. Commands should be run through the
`./bazelw` wrapper script from the main Modular repository root.

### Essential Build Commands

```bash
# Build all kernels
./bazelw build //max/kernels/...

# Build a specific module
./bazelw build //max/kernels/src/linalg:linalg

# Build a specific benchmark
./bazelw build //max/kernels/benchmarks:gpu/linalg/bench_matmul

# Build and run a benchmark
./bazelw run //max/kernels/benchmarks:gpu/linalg/bench_matmul

# Run a specific test
./bazelw test //max/kernels/test/linalg:test_matmul

# Run all tests in a directory
./bazelw test //max/kernels/test/linalg/...

# Run GPU tests with specific hardware
./bazelw test --config=remote-b200 //max/kernels/test/gpu/...
```

</details>
