---
name: esbmc__esbmc
source: https://github.com/esbmc/esbmc/blob/3b6cb6558d4825550a9afb8fe5325a02cf31440a/CLAUDE.md
repo: esbmc/esbmc
kind: claude-md
stars: 488
last_pushed: 2026-06-14T20:57:15Z
license: other
score: 9
domains: [systems-programming, formal-verification, cli-tools]
tags: [build-system, testing-rigor, agent-guidance]
curated: 2026-06-15
curated_by: config-scout
---

# esbmc/esbmc — claude-md

**Why it's worth keeping:** The 'Post-implementation Pass' workflow and the highly specific guardrails against in-tree builds or unmanaged /tmp growth are excellent templates for preventing agent errors in heavy systems code.

**Summary:** Provides extremely high-fidelity instructions for a complex C++ system, including specific warnings about build directory pollution and disk space management.

**Source credibility:** High; ESBMC is an active, established tool for formal verification.

**Recency:** Current; uses advanced agentic patterns like specialized subagents and structured verification loops.

**Source:** [esbmc/esbmc/CLAUDE.md](https://github.com/esbmc/esbmc/blob/3b6cb6558d4825550a9afb8fe5325a02cf31440a/CLAUDE.md) · 488★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AGENTS.md

This file provides guidance to coding agents working with this repository. The same workflow rules also live in `CLAUDE.md` (which Claude Code loads automatically); update both files together when changing build, test, style, or post-implementation rules.

## Project Overview

ESBMC (Efficient SMT-based Context-Bounded Model Checker) is a software model checker that detects bugs or proves their absence in C, C++, CUDA, CHERI-C, Python, Solidity, Java, and Kotlin programs. It works by parsing source → building AST → converting to GOTO program → symbolic execution (SSA) → encoding as SMT formula → solving with SMT solvers.

## Build Commands

**NEVER run cmake in the repo root (e.g., `cmake .` or `cmake -B. -S.`).** Always use `build/` or a subdirectory of it as the build directory (e.g., `-Bbuild`). The `.gitignore` only covers `build/` — in-tree builds pollute the source tree with hundreds of untracked artifacts.

```sh
# Minimal build with Z3 solver (at least one solver must be enabled for regression tests)
cmake -GNinja -Bbuild -S . \
  -DDOWNLOAD_DEPENDENCIES=On \
  -DENABLE_PYTHON_FRONTEND=On \
  -DENABLE_Z3=On \
  -DBUILD_TESTING=On \
  -DENABLE_REGRESSION=On \
```

</details>
