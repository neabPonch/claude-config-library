---
name: x402agent__solana-clawd__claude
source: https://github.com/x402agent/solana-clawd/blob/ad578b1aed8bfdff3eca8d535556bdab635907d2/agents/skills/solana-formal-verification/claude.md
repo: x402agent/solana-clawd
kind: claude-md
stars: 23
last_pushed: 2026-06-03T20:44:38Z
license: mit
score: 9
domains: [blockchain, formal-verification, rust, solana]
tags: [lean4, verifiable-ai, solana, expert-guidance]
curated: 2026-06-15
curated_by: config-scout
---

# x402agent/solana-clawd — claude-md

**Why it's worth keeping:** Includes highly specific tactical patterns (e.g., 'unfold' vs 'simp') and debugging heuristics that are critical for navigating cryptic formal proof errors. It also provides design-level rationale to align AI behavior with the project's philosophy.

**Summary:** A deep technical guide for performing formal verification of Solana programs using Lean 4 and a custom CLI tool (QEDGen).

**Source credibility:** High-quality, domain-expert documentation for a specialized tool.

**Recency:** Current; last updated within the month.

**Source:** [x402agent/solana-clawd/agents/skills/solana-formal-verification/claude.md](https://github.com/x402agent/solana-clawd/blob/ad578b1aed8bfdff3eca8d535556bdab635907d2/agents/skills/solana-formal-verification/claude.md) · 23★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

QEDGen is a Claude Code skill for formally verifying Solana programs using Lean 4 proofs. Claude (the local LLM) drives proof writing directly — reading code, writing Lean models/theorems/proofs, and iterating on `lake build` errors. Leanstral (Mistral's theorem prover) is called only for hard sub-goals via `fill-sorry`.

**Core workflow**: Claude reads source → writes SPEC.md → writes Lean 4 proofs → `lake build` → iterates → calls `qedgen fill-sorry` for hard sub-goals

## Build and Development Commands

### Build the CLI

```bash
# Build qedgen binary (outputs to ./bin/qedgen)
cargo build --release

# Build just the Lean support library
cd crates/qedgen/lean_support
lake build
```

### Run Tests

```bash
# Rust unit tests
cargo test

# Test Lean support library axioms
cd crates/qedgen/lean_support
lake env lean test_lemmas.lean

# Build the example escrow verification
cd example/escrow/formal_verification
lake build                # Verify all proofs compile
```

### QEDGen Commands

```bash
# Set up global validation workspace (first time: 15-45 min
```

</details>
