---
name: d-krupke__CheckMyTex
source: https://github.com/d-krupke/CheckMyTex/blob/7c89349a14306491b72c50a34117bb7592f6719d/CLAUDE.md
repo: d-krupke/CheckMyTex
kind: claude-md
stars: 15
last_pushed: 2026-06-15T22:14:29Z
license: mit
score: 9
domains: [cli-tools, python]
tags: [extensibility, architecture-pattern, boilerplate]
curated: 2026-06-16
curated_by: config-scout
---

# d-krupke/CheckMyTex — claude-md

**Why it's worth keeping:** The inclusion of boilerplate/templates for new classes (Checker/Filter) and a clear data-flow diagram allows Claude to perform complex feature extensions with minimal guidance.

**Summary:** Provides deep architectural context and explicit coding patterns for extending the tool's checker and filter pipelines.

**Source credibility:** A highly specialized niche project with exceptionally high-quality, recent documentation.

**Recency:** Extremely current; updated within the last month.

**Source:** [d-krupke/CheckMyTex/CLAUDE.md](https://github.com/d-krupke/CheckMyTex/blob/7c89349a14306491b72c50a34117bb7592f6719d/CLAUDE.md) · 15★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

CheckMyTex is a CLI tool for checking complex LaTeX documents (dissertations, papers) for spelling, grammar, and LaTeX-specific errors. It combines multiple checking tools (aspell/pyspellchecker, LanguageTool, ChkTeX, Proselint) with a unified interface and sophisticated whitelisting system.

**Key Design Philosophy:**
- Work on whole documents, not individual files
- Provide exact problem locations with file paths and line numbers
- Support interactive CLI workflow with vim/nano integration
- Allow whitelisting of false positives (`.whitelist.txt`)
- Support both CLI and web interfaces

## Development Commands

### Testing
```bash
# Run all tests
pytest

# Run with coverage
pytest --cov=checkmytex --cov-report=term-missing

# Run specific test file
pytest tests/test_line_length_checker.py

# Run tests across Python versions
tox
```

### Linting and Formatting
```bash
# Lint with ruff
ruff check .

# Format with ruff
ruff format .

# Type check with mypy
mypy checkmytex tests

# Run pre-commit hooks manually
pre-commit run --all-files
```

### Ru
```

</details>
