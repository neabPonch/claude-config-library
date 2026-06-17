---
name: lashex__flask-neo4j
source: https://github.com/lashex/flask-neo4j/blob/77baf6a4f08306c318afad35179957a4059517bd/CLAUDE.md
repo: lashex/flask-neo4j
kind: claude-md
stars: 57
last_pushed: 2026-03-30T20:16:27Z
license: mit
score: 8
domains: [backend-api, python]
tags: [flask, neo4j, uv]
curated: 2026-06-16
curated_by: config-scout
---

# lashex/flask-neo4j — claude-md

**Why it's worth keeping:** The Architecture section maps the API surface and configuration patterns without requiring full-repo scans. It also explicitly distinguishes between unit and integration testing requirements to prevent execution errors.

**Summary:** Provides high-density structural context and command sets for a modern Python toolchain using uv.

**Source credibility:** A specialized, well-maintained niche library with moderate star count.

**Recency:** Very current; uses the modern 'uv' toolchain and follows contemporary developer workflows.

**Source:** [lashex/flask-neo4j/CLAUDE.md](https://github.com/lashex/flask-neo4j/blob/77baf6a4f08306c318afad35179957a4059517bd/CLAUDE.md) · 57★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Flask-Neo4j is a Flask extension providing integration with Neo4j graph database via the official `neo4j` Python driver (v5.x). It supports direct and application factory initialization patterns.

## Commands

```bash
# Install dependencies
uv sync --extra dev              # Dev dependencies (testing, linting, type checking)
uv sync --extra docs             # Documentation dependencies

# Testing
uv run pytest -v -m "not integration"   # Unit tests only (mocked driver)
uv run pytest -v -m integration         # Integration tests (requires live Neo4j on localhost:7687)
uv run pytest -v                         # All tests

# Linting & formatting
uv run ruff check src/ tests/
uv run ruff format --check src/ tests/

# Type checking
uv run mypy src/

# Documentation
cd docs && uv run sphinx-build -b html . _build/html
```

## Architecture

Single-module extension in `src/flask_neo4j/extension.py` (~176 lines). The `Neo4j` class wraps `neo4j.GraphDatabase.driver()` and integrates with Flask's app context lifecycle.

**Key API surface:**
- `Neo4j(app)` o
```

</details>
