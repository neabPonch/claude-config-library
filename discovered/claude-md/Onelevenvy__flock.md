---
name: Onelevenvy__flock
source: https://github.com/Onelevenvy/flock/blob/75251629489c1f82559210ecb6930ebb97bdeaa6/CLAUDE.md
repo: Onelevenvy/flock
kind: claude-md
stars: 1072
last_pushed: 2026-06-15T07:18:11Z
license: apache-2.0
score: 9
domains: [rust, agents-ai, desktop-app]
tags: [architecture-mapping, system-logic, fullstack-tauri]
curated: 2026-06-15
curated_by: config-scout
---

# Onelevenvy/flock — claude-md

**Why it's worth keeping:** The technical mapping of high-level logic patterns (e.g., Agent Engine vs. Workflow Engine) and explicit end-to-end data flow paths are highly transferable techniques for complex repositories.

**Summary:** A comprehensive architectural blueprint for a multi-agent system that maps complex crate relationships and data flow. It provides deep context on how the engine, tools, and UI interact.

**Source credibility:** Highly credible; a highly starred repository with recent maintenance activity.

**Recency:** Extremely current, referencing modern tech like Rust 2024 and updated toolchains.

**Source:** [Onelevenvy/flock/CLAUDE.md](https://github.com/Onelevenvy/flock/blob/75251629489c1f82559210ecb6930ebb97bdeaa6/CLAUDE.md) · 1072★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Flock is a multi-provider AI agent desktop application with tool orchestration, sandbox execution, visual workflow, and browser/computer-use capabilities. It's a Rust workspace with a Tauri-based desktop UI (React + TypeScript + Mantine).

## Build & Development Commands

### Rust Backend
```bash
# Build the CLI
cargo build --release

# Run in single-shot mode
cargo run -- "your question"

# Run interactive REPL
cargo run

# Run with specific provider/profile
cargo run -- --profile deepseek "your question"

# Run tests (workspace-wide)
cargo test

# Run a single crate's tests
cargo test -p flock-core
cargo test -p flock-agent
cargo test -p flock-tools
cargo test -p flock-skills

# Run a specific test
cargo test -p flock-core test_name

# Lint
cargo clippy --workspace
```

### Tauri Desktop UI
```bash
cd flock-ui

# Install dependencies
npm install

# Development server
npm run dev
# or
npm run tauri dev

# Build for production
npm run build
# or
npm run tauri build

# Lint frontend
npm run lint
```

## Architecture

### Workspace Crates

| Crate
```

</details>
