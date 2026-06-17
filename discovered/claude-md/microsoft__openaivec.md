---
name: microsoft__openaivec
source: https://github.com/microsoft/openaivec/blob/b60d1270edcdafa2b8352ac04701afad0f741274/CLAUDE.md
repo: microsoft/openaivec
kind: claude-md
stars: 25
last_pushed: 2026-06-12T22:18:16Z
license: mit
score: 9
domains: [data-science, python-library, backend]
tags: [python, typing-strict, uv-tooling]
curated: 2026-06-15
curated_by: config-scout
---

# microsoft/openaivec — claude-md

**Why it's worth keeping:** The 'Code Style Guidelines' section is exceptional; it provides granular instructions on modern Python type syntax and dependency injection patterns to prevent the AI from using legacy conventions.

**Summary:** A comprehensive guide that combines technical architecture, specific toolchain commands using uv/ruff, and rigorous coding standards.

**Source credibility:** High-quality specialized library with very recent maintenance activity.

**Recency:** Extremely current, utilizing modern standards like uv, ruff, and PEP 604 union types.

**Source:** [microsoft/openaivec/CLAUDE.md](https://github.com/microsoft/openaivec/blob/b60d1270edcdafa2b8352ac04701afad0f741274/CLAUDE.md) · 25★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is **openaivec**, a Python library that enables AI-powered text processing at scale for pandas DataFrames and Apache Spark. The project provides vectorized OpenAI API access, reducing latency and API costs through batch processing and automatic deduplication.

## Development Commands

### Dependencies and Environment
```bash
# Install all dependencies (development and optional extras)
uv sync --all-extras --dev

# Install package in development mode
uv pip install -e .
```

### Code Quality and Testing
```bash
# Run linting and formatting (check, auto-fix, and format)
uv run ruff check . --fix && uv run ruff format .

# Run tests
uv run pytest

# Run tests for a specific module
uv run pytest tests/test_[module_name].py
```

### Documentation
```bash
# Build and serve documentation locally (uses MkDocs)
uv run mkdocs serve

# Build documentation for deployment
uv run mkdocs build
```

## Architecture and Structure

### Core Components

- **BatchResponses/AsyncBatchResponses** (`src/openaivec/responses.py`): Vectorized API interface for OpenAI
```

</details>
