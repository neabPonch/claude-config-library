---
name: DHI__mikeio
source: https://github.com/DHI/mikeio/blob/f5300ca61c477ae7bff0b5c0e2213fe84c0da7cc/CLAUDE.md
repo: DHI/mikeio
kind: claude-md
stars: 180
last_pushed: 2026-06-04T07:45:11Z
license: bsd-3-clause
score: 10
domains: [scientific-computing, data-engineering, python]
tags: [architecture-mapping, domain-knowledge, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# DHI/mikeio — claude-md

**Why it's worth keeping:** It provides explicit mental models via 'Design Patterns' and 'Data Flow Patterns,' and includes low-level technical specs (like 1-based indexing) crucial for preventing logic errors in scientific computing.

**Summary:** This file acts as a comprehensive knowledge base that combines project setup instructions with deep domain-specific data specifications.

**Source credibility:** High; the repository is a mature, well-maintained tool with significant stars used in hydrological modeling.

**Recency:** Very current, utilizing modern standards like 'uv' and 'ruff'.

**Source:** [DHI/mikeio/CLAUDE.md](https://github.com/DHI/mikeio/blob/f5300ca61c477ae7bff0b5c0e2213fe84c0da7cc/CLAUDE.md) · 180★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

MIKE IO is a Python package for reading, writing, and manipulating MIKE files (dfs0, dfs1, dfs2, dfs3, dfsu, mesh). It provides a high-level API for common data processing workflows with MIKE files from DHI.

## Development Commands

### Setup
```bash
# Install package in editable mode with dev dependencies
uv sync --group dev

# Or install all dependency groups (dev, test, notebooks)
uv sync --all-groups
```

### Testing
```bash
# Run all tests (excludes performance and notebook tests by default)
uv run pytest

# Run tests with coverage
uv run pytest --cov-report html --cov=mikeio tests/

# Run specific test file
uv run pytest tests/test_dfs0.py

# Run specific test function
uv run pytest tests/test_dfs0.py::test_repr

# Run performance tests
uv run pytest tests/performance/ --durations=0
```

### Code Quality
```bash
# Run all checks (lint, typecheck, test)
just check

# Lint code
uv run ruff check .

# Format code (required before committing)
uv run ruff format .

# Type checking
uv run mypy .
```

### Building
```bash
# Build package (include
```

</details>
