---
name: amphibian-dev__toad
source: https://github.com/amphibian-dev/toad/blob/d4e991724e2f7aa535c18e96ef6f406609a881f9/CLAUDE.md
repo: amphibian-dev/toad
kind: claude-md
stars: 526
last_pushed: 2026-05-21T03:22:47Z
license: mit
score: 9
domains: [data-science, machine-learning, python, rust]
tags: [hybrid-language, build-systems, scikit-learn, technical-documentation]
curated: 2026-06-15
curated_by: config-scout
---

# amphibian-dev/toad — claude-md

**Why it's worth keeping:** The 'Rust Components' section is vital for preventing errors when modifying native extensions; the 'Typical Workflow' provides high-level semantic context for complex task execution.

**Summary:** A highly detailed guide for a hybrid Python/Rust repository that explains module responsibilities and specialized build requirements.

**Source credibility:** Strong; a well-maintained, starred open-source project (ESC Team).

**Recency:** 

**Source:** [amphibian-dev/toad/CLAUDE.md](https://github.com/amphibian-dev/toad/blob/d4e991724e2f7aa535c18e96ef6f406609a881f9/CLAUDE.md) · 526★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Toad is a Python package for scorecard model development, particularly focused on credit scoring and risk modeling. It provides tools for the entire modeling pipeline: EDA, feature engineering, feature selection, binning, model validation, and scorecard transformation.

**Key characteristics:**
- Python 3.9+ required
- **Uses Rust (via PyO3/maturin) for performance-critical binning/merging algorithms**
- Scikit-learn compatible transformers and estimators
- Supports both Chinese and English documentation

## Build and Development Commands

### Setup and Installation

**Prerequisites:**
- Rust toolchain (install with: `curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh`)
- Python 3.9+

```bash
make install          # Install package in development mode (builds Rust extensions first)
make build           # Build Rust extensions using maturin
make build_deps      # Install build dependencies (including maturin)
```

**Alternative build methods:**
```bash
# Using maturin directly (requires virtualenv)
maturin develop --release

# Or build
```

</details>
