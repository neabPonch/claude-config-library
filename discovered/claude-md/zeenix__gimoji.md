---
name: zeenix__gimoji
source: https://github.com/zeenix/gimoji/blob/3577ae07e0cb68674a7935d5d43ad9a1a7d460d5/CLAUDE.md
repo: zeenix/gimoji
kind: claude-md
stars: 52
last_pushed: 2026-06-09T17:37:39Z
license: mit
score: 8
domains: [cli-tools, rust]
tags: [cli, rust, architecture]
curated: 2026-06-14
curated_by: config-scout
---

# zeenix/gimoji — claude-md

**Why it's worth keeping:** The inclusion of the 'Build Process' section explains compile-time logic (build.rs), which prevents an agent from making incorrect assumptions about data loading. The 'Architecture' section effectively maps files to their specific responsibilities.

**Summary:** Provides a clear map of project structure and essential build/test commands for a Rust CLI tool.

**Source credibility:** A well-maintained, specialized CLI tool with a clear purpose.

**Recency:** Current and follows modern patterns for LLM-assisted development.

**Source:** [zeenix/gimoji/CLAUDE.md](https://github.com/zeenix/gimoji/blob/3577ae07e0cb68674a7935d5d43ad9a1a7d460d5/CLAUDE.md) · 52★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this
repository.

## Project Overview

Gimoji is a Rust CLI tool for adding emojis to git commit messages. It provides a terminal UI for
emoji selection and integrates with git as a prepare-commit-msg hook.

## Development Commands

- **Build**: `cargo build` or `cargo build --release`
- **Run**: `cargo run` (launches emoji picker UI)
- **Run with args**: `cargo run -- --help` (see all options)
- **Test**: `cargo test`
- **Install locally**: `cargo install --path .`
- **Format code**: `cargo fmt`
- **Lint**: `cargo clippy`

## Architecture

### Core Components

- **main.rs**: Entry point with CLI argument parsing, hook installation, and main application flow
- **emoji.rs**: Emoji data structure and search functionality. Contains pre-compiled emoji database
  from emojis.json
- **terminal.rs**: Terminal setup and management using crossterm/ratatui
- **selection_view.rs**: Grid-based emoji selection UI component
- **search_entry.rs**: Text search input component with filtering
- **colors.rs**: Color scheme definitions for light/dark terminal themes

### Key Features

- Full-screen termi
```

</details>
