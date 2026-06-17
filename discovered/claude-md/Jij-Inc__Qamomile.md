---
name: Jij-Inc__Qamomile
source: https://github.com/Jij-Inc/Qamomile/blob/0aaef41fe2d12453d53b52e221ba193279177f01/CLAUDE.md
repo: Jij-Inc/Qamomile
kind: claude-md
stars: 18
last_pushed: 2026-06-12T07:34:32Z
license: apache-2.0
score: 9
domains: [compiler-design, quantum-computing, systems-programming]
tags: [architecture, pipeline, low-level]
curated: 2026-06-15
curated_by: config-scout
---

# Jij-Inc/Qamomile — claude-md

**Why it's worth keeping:** It defines specific 'don't do this' design principles to prevent structural regressions and maps out a complex state-machine/pipeline flow that guides code placement.

**Summary:** Provides rigorous architectural constraints and detailed compiler pipeline stages for a quantum programming language.

**Source credibility:** High; the depth of the technical documentation suggests it was written by experienced systems/compiler engineers.

**Recency:** Current; utilizes modern Python tooling like uv, ruff, and zuban.

**Source:** [Jij-Inc/Qamomile/CLAUDE.md](https://github.com/Jij-Inc/Qamomile/blob/0aaef41fe2d12453d53b52e221ba193279177f01/CLAUDE.md) · 18★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build and Development Commands

```bash
# Install dependencies (using uv)
uv sync

# Run all tests
uv run pytest tests/

# Unit tests only (default, skips docs)
uv run pytest

# Docs tests only
uv run pytest -m docs -v

# All tests (unit + docs)
uv run pytest -m "" -v

# Specific tutorial
uv run pytest -m docs -k "en/tutorial/qaoa" -v

# Run a single test file
uv run pytest tests/core/test_qaoa.py

# Run a specific test
uv run pytest tests/core/test_qaoa.py::test_qaoa_converter -v

# Lint and isort with ruff
uv run ruff check qamomile/

# Format with ruff
uv run ruff format qamomile/

# Type checking with zuban
uv run zuban check qamomile/

# Build documentation (from docs/en or docs/ja directory)
jupyter-book build .
```

## Architecture Overview

Qamomile is a quantum programming language built around a circuit-first compiler core. The central abstraction is `@qkernel`: users write quantum programs in Python, and the compiler pipeline transforms them into executable circuits for multiple backends.

### Design Center

**`qamomile.circuit`** is the compiler core.
```

</details>
