---
name: vincentarelbundock__marginaleffects__claude
source: https://github.com/vincentarelbundock/marginaleffects/blob/863b62a5fb302e8c1782cd869e58e83bc7877b7d/python/CLAUDE.md
repo: vincentarelbundock/marginaleffects
kind: claude-md
stars: 616
last_pushed: 2026-06-01T03:51:12Z
license: unknown
score: 9
domains: [data-science, python, statistics]
tags: [architecture, testing, data-flow, uv]
curated: 2026-06-15
curated_by: config-scout
---

# vincentarelbundock/marginaleffects — claude-md

**Why it's worth keeping:** It explains the 'logic' of the system (e.g., function delegation and the 'vault' pattern) rather than just listing files. This allows an AI to understand how new features should integrate into existing pipelines.

**Summary:** Provides a deep technical mental model of the software architecture, including data flow patterns and structural dependencies. Includes highly actionable CLI shortcuts using modern tooling like `uv`.

**Source credibility:** High; based on a popular, actively maintained statistical R package with a Python port.

**Recency:** 

**Source:** [vincentarelbundock/marginaleffects/python/CLAUDE.md](https://github.com/vincentarelbundock/marginaleffects/blob/863b62a5fb302e8c1782cd869e58e83bc7877b7d/python/CLAUDE.md) · 616★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Quick Reference

```bash
# From repo root (preferred — handles install before test):
make py-test           # Install + run full test suite (parallel)
make py-lint           # ruff check + format
make py-install        # Install package (editable)

# From python/ directory:
uv run --all-extras pytest tests/test_predictions.py              # Single test file
uv run --all-extras pytest tests/test_predictions.py::test_name -v  # Single test
uv run --all-extras ruff check marginaleffects                    # Lint only
uv run --all-extras ruff format marginaleffects tests             # Format only
```

## Setup

```bash
uv venv .venv
source .venv/bin/activate
uv pip install -e .          # Editable install
uv pip install -e ".[test]"  # With test dependencies
```

## Architecture Overview

Python package for statistical marginal effects analysis. Unified interface for predictions, comparisons, and slopes across modeling frameworks. Docs: https://marginaleffects.com/

### Core Pipeline

The three main functions (`predictions()`, `comparisons()`, `slopes()`) share a comm
```

</details>
