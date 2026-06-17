---
name: FolhaSP__mosaico
source: https://github.com/FolhaSP/mosaico/blob/b3c2a5e6ed21ebdabf955c519d66a458c2bd08e4/CLAUDE.md
repo: FolhaSP/mosaico
kind: claude-md
stars: 18
last_pushed: 2025-12-03T20:36:34Z
license: gpl-3.0
score: 9
domains: [cli-tools, media-processing, python]
tags: [architecture-driven, data-flow, modern-python]
curated: 2026-06-16
curated_by: config-scout
---

# FolhaSP/mosaico — claude-md

**Why it's worth keeping:** The use of an ASCII data flow diagram and explicit 'Extension Points' provides critical context for an AI to write compatible code without violating existing abstractions.

**Summary:** Combines essential developer commands with a deep architectural mental model of the system's data flow and design patterns.

**Source credibility:** A specialized open-source video framework with high-quality, structured documentation.

**Recency:** Very current; uses modern standards like uv, ruff, and type-hinted protocols.

**Source:** [FolhaSP/mosaico/CLAUDE.md](https://github.com/FolhaSP/mosaico/blob/b3c2a5e6ed21ebdabf955c519d66a458c2bd08e4/CLAUDE.md) · 18★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Package Management
- **Install dependencies**: `make install` (installs all dependencies and pre-commit hooks via uv)
- **Sync dependencies**: `uv sync --frozen --all-extras`

### Code Quality
- **Lint code**: `make lint` or `uv run ruff check . --fix`
- **Format code**: `make format` or `uv run ruff format .`
- **Run all quality checks**: `make all` (lint + format + test)

### Testing
- **Run unit tests**: `make test` or `uv run pytest tests`
- **Run E2E tests**: `make e2e` or `uv run pytest e2e`
- **Run specific test**: `uv run pytest tests/path/to/test_file.py::test_function`

### Documentation
- **Build docs**: `make docs` or `uv run mkdocs build`
- **Serve docs locally**: `make docs-serve` or `uv run mkdocs serve --no-strict`

### CLI Usage
- **Run mosaico CLI**: `uv run mosaico` or `python -m mosaico`

## Architecture Overview

Mosaico is a Python video generation framework built on a composition-based architecture that treats video creation as orchestrating media assets on a timeline.

### Core Components

**Media Layer** (`media.p
```

</details>
