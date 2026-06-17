---
name: audulus__rui
source: https://github.com/audulus/rui/blob/365eaab98a235d552dc3e16cc7c903d9510df4c6/CLAUDE.md
repo: audulus/rui
kind: claude-md
stars: 2024
last_pushed: 2026-05-22T02:06:24Z
license: mit
score: 9
domains: [rust, ui-frameworks]
tags: [architecture-driven, system-design]
curated: 2026-06-14
curated_by: config-scout
---

# audulus/rui — claude-md

**Why it's worth keeping:** It defines the critical relationship between ViewIds, Context, and State to prevent hallucinations; it also includes specific instructions for running nested Cargo projects as integration tests.

**Summary:** Provides a deep architectural mental model of a custom reactive UI system and detailed command patterns for running specialized examples.

**Source credibility:** High-quality open-source Rust project with significant community traction (2k+ stars).

**Recency:** Current; reflects modern development patterns.

**Source:** [audulus/rui/CLAUDE.md](https://github.com/audulus/rui/blob/365eaab98a235d552dc3e16cc7c903d9510df4c6/CLAUDE.md) · 2024★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

rui is an experimental declarative UI library for Rust, inspired by SwiftUI. It focuses on GPU-rendered UIs that update reactively when state changes, without a retained view tree or DOM diffing. The entire UI is re-rendered when state changes, under the assumption that this is fast enough for good performance.

## Common Development Commands

### Building and Testing
- `cargo build` - Build the project
- `cargo test` - Run tests
- `cargo check` - Check for compilation errors without building

### Running Examples
- `cargo run --example <example_name>` - Run a specific example (e.g., `counter`, `shapes`, `canvas`, `slider`, `gallery`)
- `cd examples/<example_name> && cargo run` - For examples with their own Cargo.toml (calculator, synth, flip_cards)

Key examples:
- `cargo run --example counter` - Basic counter demo
- `cargo run --example gallery` - Widget gallery showing all components
- `cargo run --example shapes` - Basic shapes rendering
- `cargo run --example canvas` - GPU vector graphics with vger
- `cd examples/calculator && cargo run` - C
```

</details>
