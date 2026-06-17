---
name: mickvangelderen__micrograd-rs-digits
source: https://github.com/mickvangelderen/micrograd-rs-digits/blob/a19b5d6bacee3574f4afa7f27dd6ad316913b742/CLAUDE.md
repo: mickvangelderen/micrograd-rs-digits
kind: claude-md
stars: 1
last_pushed: 2025-10-03T00:30:53Z
license: unknown
score: 7
domains: [machine-learning, cli-tools]
tags: [rust, performance-focused, opinionated-style]
curated: 2026-06-15
curated_by: config-scout
---

# mickvangelderen/micrograd-rs-digits — claude-md

**Why it's worth keeping:** The style guidelines use specific technical constraints (e.g., preference for trait generics over slices) instead of generic platitudes, which helps guide LLM coding patterns effectively.

**Summary:** Provides performance-aware build instructions and highly opinionated Rust development guidelines.

**Source credibility:** Low-star educational/example repository.

**Recency:** Current; aligns well with modern Rust and Claude Code workflows.

**Source:** [mickvangelderen/micrograd-rs-digits/CLAUDE.md](https://github.com/mickvangelderen/micrograd-rs-digits/blob/a19b5d6bacee3574f4afa7f27dd6ad316913b742/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Description

This project is an example project training a neural network on the scikit learn digits dataset using [micrograd-rs](https://github.com/mickvangelderen/micrograd-rs).

The micrograd-rs library we are compiling against might be available at a local path if `./patch.bash` is has been applied.

## Commands

### Building and running the application

The application performs a reasonable amount of computation and compiling in release mode provides a significant speed up.

```bash
cargo run --release -- <args...>
```

The application should output an up-to-date help page when not passing any argyments.

### Formatting, linting and testing

```
./ci.bash
```

### Determining the source of a package

This can be used to, for example, determine if `micrograd-rs` is being build from a local path or the git directory.

```bash
cargo tree --quiet --offline --package <package>
```

## Software Development Guidelines

The author of this project cares about code quality.
The following is a list of guidelines that should be respected.
This list is just a sele
```

</details>
