---
name: widgetti__solara
source: https://github.com/widgetti/solara/blob/4804a0e4e711a70ed243b470f633999d897637d8/CLAUDE.md
repo: widgetti/solara
kind: claude-md
stars: 2163
last_pushed: 2026-06-09T14:49:03Z
license: mit
score: 9
domains: [python, web-frameworks, devops]
tags: [dev-workflow, testing-patterns, ci-cd]
curated: 2026-06-15
curated_by: config-scout
---

# widgetti/solara — claude-md

**Why it's worth keeping:** It includes highly specific 'how-to' snippets for component testing, explains how to interpret flaky CI failures, and details a rigorous branching/squashing strategy.

**Summary:** This file provides comprehensive project context including specific testing patterns, development toolchains (uv), and detailed Git/GitHub CLI workflows.

**Source credibility:** High: 2k+ stars and very recent active maintenance.

**Recency:** Current; utilizes modern tooling like uv and gh CLI commands.

**Source:** [widgetti/solara/CLAUDE.md](https://github.com/widgetti/solara/blob/4804a0e4e711a70ed243b470f633999d897637d8/CLAUDE.md) · 2163★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance for Claude Code (claude.ai/claude-code) when working with this repository.

## Project Overview

Solara is a pure Python, React-style framework for building Jupyter and web applications. It uses a React-like API with ipywidgets, enabling component-based code and simple state management. Apps work both inside Jupyter Notebook and as standalone web apps.

## Repository Structure

- `solara/` - Main source code
  - `components/` - UI components (Button, FileBrowser, etc.)
  - `server/` - Solara server implementation
  - `hooks/` - React-style hooks (use_state, use_effect, etc.)
  - `website/` - Documentation website
- `tests/` - Test suite
  - `unit/` - Unit tests
  - `integration/` - Integration tests
- `packages/` - Sub-packages (solara-server, solara-enterprise, etc.)

## Development Commands

### Setting Up the Development Environment

Use `uv` to create a virtual environment and install dependencies:

```bash
# Create venv with Python 3.11
uv venv .venv --python 3.11

# Install all dev dependencies
uv pip install -r requirements-dev.txt --python .venv/bin/python
```

### Running Tests

```bash
# Run all unit tests
uv run pytest tests/unit/
```

</details>
