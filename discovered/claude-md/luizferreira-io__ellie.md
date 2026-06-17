---
name: luizferreira-io__ellie
source: https://github.com/luizferreira-io/ellie/blob/928085e2e0a2a6f684cf277208ae1ba7d1939c5f/CLAUDE.md
repo: luizferreira-io/ellie
kind: claude-md
stars: 23
last_pushed: 2026-05-19T21:00:53Z
license: gpl-3.0
score: 9
domains: [cli-tools, rust]
tags: [tui, architecture-pattern, system-programming]
curated: 2026-06-15
curated_by: config-scout
---

# luizferreira-io/ellie — claude-md

**Why it's worth keeping:** It includes specific runtime arguments for 'cargo run', enforces coding standards (like color palette usage), and explains complex state patterns like the MetricHistory ring buffer.

**Summary:** Provides a deep architectural breakdown of the trait-based UI system and detailed execution commands for a Rust TUI tool.

**Source credibility:** A specialized PostgreSQL tool with recent maintenance activity.

**Recency:** Very current, specifically mentioning Rust 2024 edition.

**Source:** [luizferreira-io/ellie/CLAUDE.md](https://github.com/luizferreira-io/ellie/blob/928085e2e0a2a6f684cf277208ae1ba7d1939c5f/CLAUDE.md) · 23★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Ellie is a terminal-based PostgreSQL performance monitoring and tuning tool built in Rust. It connects to a PostgreSQL server and renders a real-time TUI dashboard using [ratatui](https://github.com/ratatui-org/ratatui).

## Commands

```bash
# Build (debug)
cargo build

# Build (release, optimized)
cargo build --release

# Build for musl (portable Linux binary)
cargo build --release --target x86_64-unknown-linux-musl

# Run tests
cargo test

# Run a single test by name
cargo test <test_name>

# Lint
cargo clippy

# Run (requires a running PostgreSQL server)
cargo run -- --host localhost --port 5432 --user postgres --password postgres --database postgres
cargo run -- --url postgresql://user:pass@host:5432/dbname
```

MSRV: **1.85** (Rust 2024 edition).

## Architecture

### Entry point and main loop

`main.rs` installs a panic hook that restores the terminal before printing, then delegates to `App::new().init().run()`.

`app.rs` — `App` owns:
- A `Vec<Box<dyn Tab>>` with all six tabs (Dashboard, Activity, Settings, File Settings, Tuning, About)
-
```

</details>
