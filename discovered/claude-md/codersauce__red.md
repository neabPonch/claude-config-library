---
name: codersauce__red
source: https://github.com/codersauce/red/blob/9dc6f3881a119998c0efea24146322ef30daa604/CLAUDE.md
repo: codersauce/red
kind: claude-md
stars: 160
last_pushed: 2026-06-14T19:47:29Z
license: mit
score: 9
domains: [cli-tools, rust]
tags: [architecture, systems, plugin-api]
curated: 2026-06-15
curated_by: config-scout
---

# codersauce/red — claude-md

**Why it's worth keeping:** It provides a mental model of the system by explicitly linking core concepts (like the state machine or buffer management) to specific source files. The inclusion of a plugin API example is highly effective for helping an agent write extensibility code.

**Summary:** Combines essential build/test commands with rich architectural mapping and design pattern descriptions.

**Source credibility:** High; based on a specialized, well-structured Rust project with clear intent.

**Recency:** Current; follows modern best practices for providing high-context guidance to AI agents.

**Source:** [codersauce/red/CLAUDE.md](https://github.com/codersauce/red/blob/9dc6f3881a119998c0efea24146322ef30daa604/CLAUDE.md) · 160★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

### Build and Run
```bash
# Build the project
cargo build

# Build release version
cargo build --release

# Run the editor
cargo run -- <file>

# Install locally
cargo install --path .
```

### Testing
```bash
# Run all tests
cargo test

# Run a specific test
cargo test test_name

# Run tests with output
cargo test -- --nocapture
```

### Development
```bash
# Check code without building
cargo check

# Format code (if rustfmt is configured)
cargo fmt

# Run linter (if clippy is configured)
cargo clippy
```

## Architecture

Red is a modal text editor built in Rust, inspired by Vim. The codebase follows an event-driven architecture with async programming using tokio.

### Core Components

- **Editor State Machine**: The editor operates in different modes (Normal, Insert, Visual, Command). Mode transitions are handled in `src/editor.rs`.

- **Buffer Management**: Text is stored using the Ropey rope data structure for efficient manipulation. See `src/buffer.rs`.

- **Language Server Protocol**: LSP client implementation in `src/lsp/` provides IDE features.
```

</details>
