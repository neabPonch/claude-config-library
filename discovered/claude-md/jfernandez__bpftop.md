---
name: jfernandez__bpftop
source: https://github.com/jfernandez/bpftop/blob/adc18f432feb485a3e999fa2d8d6f1658d76e2ac/CLAUDE.md
repo: jfernandez/bpftop
kind: claude-md
stars: 2687
last_pushed: 2026-06-03T06:38:36Z
license: apache-2.0
score: 9
domains: [cli-tools, systems-programming, rust]
tags: [rust, ebpf, tui]
curated: 2026-06-16
curated_by: config-scout
---

# jfernandez/bpftop — claude-md

**Why it's worth keeping:** Provides strict safety conventions for `unsafe` blocks and clearly explains the build-time generation of BPF skeletons to prevent manual editing of generated files.

**Summary:** Defines precise workflows for a complex Rust + eBPF toolchain, including specific commands and architectural context.

**Source credibility:** High; highly starred (2.6k+) and actively maintained systems tool.

**Recency:** Very recent, following modern Rust/eBPF best practices.

**Source:** [jfernandez/bpftop/CLAUDE.md](https://github.com/jfernandez/bpftop/blob/adc18f432feb485a3e999fa2d8d6f1658d76e2ac/CLAUDE.md) · 2687★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

bpftop is a dynamic real-time view of running eBPF programs written in Rust. It displays runtime statistics, events per second, and CPU utilization for eBPF programs, using a TUI (Terminal User Interface) built with ratatui.

## Development Commands

### Building
```bash
cargo build --release
```

### Testing
```bash
cargo test
```

### Code Quality
```bash
cargo clippy --all --tests --all-features --no-deps
```

### Running
```bash
# Run the application (requires sudo privileges)
sudo ./target/release/bpftop
```

## Architecture

### Core Components

1. **Main Entry** (`src/main.rs`): Handles initialization, terminal setup, main event loop, and BPF statistics collection using `BPF_ENABLE_STATS` syscall.

2. **Application State** (`src/app.rs`): Manages UI state, sorting, filtering, and view modes (tabular vs graph views).

3. **BPF Program Data** (`src/bpf_program.rs`): Represents individual eBPF programs with their statistics and handles data collection/calculation.

4. **BPF Integration** (`src/bpf/`):
   - `pid_iter.bpf.c`: BPF C code for ite
```

</details>
