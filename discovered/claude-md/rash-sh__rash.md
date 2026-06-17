---
name: rash-sh__rash
source: https://github.com/rash-sh/rash/blob/6d6f8420c96e9a662a2bc2bbefff84b6c324cff6/CLAUDE.md
repo: rash-sh/rash
kind: claude-md
stars: 246
last_pushed: 2026-06-13T22:43:02Z
license: gpl-3.0
score: 9
domains: [cli-tools, systems-programming, rust]
tags: [procedural-guide, rust, architecture, standards]
curated: 2026-06-15
curated_by: config-scout
---

# rash-sh/rash — claude-md

**Why it's worth keeping:** It includes actionable 'how-to' steps for adding new modules and specific negative constraints (e.g., no unwrap/expect) that prevent common AI-generated code errors.

**Summary:** Provides high-fidelity technical blueprints for extending the module system and enforces strict coding guardrails for Rust development.

**Source credibility:** High; comes from a well-structured, actively maintained Rust systems project.

**Recency:** 

**Source:** [rash-sh/rash/CLAUDE.md](https://github.com/rash-sh/rash/blob/6d6f8420c96e9a662a2bc2bbefff84b6c324cff6/CLAUDE.md) · 246★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## About Rash

Rash is a declarative shell scripting language using Ansible-like YAML syntax, compiled to a single Rust binary. It's designed for container entrypoints, IoT devices, and local scripting with zero dependencies. Scripts use `.rh` extension and are executable with `#!/usr/bin/env rash` shebang.

## Essential Commands

### Building and Testing

```bash
# IMPORTANT: Always use Make targets, never raw cargo commands
make build              # Debug build (uses cargo or cross based on target)
make release            # Release build for current platform
make test               # Lint + unit tests + integration tests (*.rh scripts)
make lint               # fmt --check + clippy -D warnings
make lint-fix           # Auto-fix formatting and clippy issues

# Cross-compilation
make release CARGO_TARGET=x86_64-unknown-linux-musl  # MUSL build
```

### Testing Specific Components

```bash
# Run specific Rust test
cargo test -p rash_core test_name

# Run specific integration test script
cargo run --bin rash test/path/to/test.rh

# Run examples (smoke tests)
make test-
```

</details>
