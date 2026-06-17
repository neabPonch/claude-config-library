---
name: jcreinhold__intensity-normalization
source: https://github.com/jcreinhold/intensity-normalization/blob/6d2e48672dc9a89fac9a0221f5be065a8dcd0727/CLAUDE.md
repo: jcreinhold/intensity-normalization
kind: claude-md
stars: 342
last_pushed: 2025-07-21T23:57:09Z
license: mit
score: 9
domains: [data-science, cli-tools, python]
tags: [clean-architecture, uv, pytest, scientific-computing]
curated: 2026-06-14
curated_by: config-scout
---

# jcreinhold/intensity-normalization — claude-md

**Why it's worth keeping:** Includes explicit 'recipes' for extending functionality (Adding New Normalizers) and specific implementation nuances like metadata preservation via `.with_data()`.

**Summary:** A highly structured guide that covers the complete development lifecycle using the `uv` toolchain and explains a Clean Architecture implementation.

**Source credibility:** The repository has significant stars (342) and follows modern Python best practices using `uv` and `ruff`.

**Recency:** Highly current, utilizing contemporary tools like `uv` that are central to modern Python workflows.

**Source:** [jcreinhold/intensity-normalization/CLAUDE.md](https://github.com/jcreinhold/intensity-normalization/blob/6d2e48672dc9a89fac9a0221f5be065a8dcd0727/CLAUDE.md) · 342★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

This project uses `uv` as the modern Python package manager. Key commands:

### Setup

```bash
# Install uv if not already installed
curl -LsSf https://astral.sh/uv/install.sh | sh

# Create virtual environment and install all dependencies
uv sync --dev
```

### Testing

```bash
# Run all tests
uv run pytest

# Run tests with coverage
uv run pytest --cov=intensity_normalization --cov-report=html

# Run specific test file
uv run pytest tests/test_normalizers.py

# Run specific test
uv run pytest tests/test_normalizers.py::TestFCMNormalizer::test_fcm_basic
```

### Code Quality

```bash
# Format code
uv run ruff format src/intensity_normalization/

# Lint code
uv run ruff check src/intensity_normalization/

# Fix linting issues automatically
uv run ruff check --fix src/intensity_normalization/

# Type checking
uv run mypy src/intensity_normalization/
```

### Building

```bash
# Build package
uv build
```

## Architecture Overview

The codebase follows Clean Architecture principles with clear separation of concerns:

### Domain Layer (`domain/`
```

</details>
