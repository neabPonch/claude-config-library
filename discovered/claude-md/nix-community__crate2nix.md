---
name: nix-community__crate2nix
source: https://github.com/nix-community/crate2nix/blob/c994c83963b42b26f127e9cc50a8c86852db67d0/CLAUDE.md
repo: nix-community/crate2nix
kind: claude-md
stars: 502
last_pushed: 2026-06-10T16:22:23Z
license: apache-2.0
score: 9
domains: [cli-tools, rust, devops]
tags: [rust, nix, build-system]
curated: 2026-06-16
curated_by: config-scout
---

# nix-community/crate2nix — claude-md

**Why it's worth keeping:** The Architecture section explains the functional pipeline of modules rather than just listing files, and Commands include specific flags for different test modes.

**Summary:** Provides a high-density technical map including environment setup, command catalogs, and module-level logic flows.

**Source credibility:** High: maintained project in a popular niche ecosystem (Nix) with strong social proof via stars.

**Recency:** Current; highly optimized for agent-based tool use and shell execution.

**Source:** [nix-community/crate2nix/CLAUDE.md](https://github.com/nix-community/crate2nix/blob/c994c83963b42b26f127e9cc50a8c86852db67d0/CLAUDE.md) · 502★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working
with code in this repository.

## Project Overview

crate2nix generates Nix build files (`Cargo.nix`) for Rust/Cargo projects,
enabling crate-by-crate hermetic builds with Nix. It reads
`Cargo.toml`/`Cargo.lock`, resolves dependencies, prefetches hashes, and
renders Nix derivations via Tera templates.

## Development Environment

The project uses a Nix flake with direnv integration. Enter the dev shell
via `direnv allow` or `nix develop`. All shell scripts (e.g., `cargo.sh`,
`run_tests.sh`) auto-enter the pure nix-shell if not already inside.

## Common Commands

### Build

```bash
nix build                            # Build crate2nix via Nix
./cargo.sh build                     # Build with cargo (inside nix-shell)
```

### Test

```bash
./run_tests.sh                       # Full test suite
./run_tests.sh --no-cargo-build      # Skip cargo build/test steps (Nix-only)
./cargo.sh test                      # Rust unit tests only
./cargo.sh test test_name            # Single Rust test
./nix-test.sh ./crate2nix/templates/nix/crate2nix/tests/default.nix
nix flake check                      # Nix inte
```

</details>
