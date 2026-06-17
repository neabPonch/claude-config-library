---
name: UKGovernmentBEIS__control-arena
source: https://github.com/UKGovernmentBEIS/control-arena/blob/3cceb4aba8f0511e47c2cf31206118b8343804b9/CLAUDE.md
repo: UKGovernmentBEIS/control-arena
kind: claude-md
stars: 201
last_pushed: 2026-06-09T16:13:40Z
license: mit
score: 9
domains: [python, async-programming, ai-security]
tags: [python, anyio, strict-typing, tooling]
curated: 2026-06-15
curated_by: config-scout
---

# UKGovernmentBEIS/control-arena — claude-md

**Why it's worth keeping:** The 'Async Code' section is exceptional; it provides explicit replacement mappings to prevent the common mistake of using asyncio primitives instead of anyio. The inclusion of documentation formatting rules (Quarto) also prevents subtle rendering bugs.

**Summary:** A highly rigorous instruction set for a Python project using uv and ruff, emphasizing strict typing and specific async concurrency patterns.

**Source credibility:** High-quality source from the UK AI Security Institute with active maintenance and a clear toolchain (uv/ruff).

**Recency:** 

**Source:** [UKGovernmentBEIS/control-arena/CLAUDE.md](https://github.com/UKGovernmentBEIS/control-arena/blob/3cceb4aba8f0511e47c2cf31206118b8343804b9/CLAUDE.md) · 201★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This repository contains code for control-arena, an open source library for AI Control experiments built on top of Inspect AI. It is built by the UK AI Security Institute.

Code can be found in `control_arena/`.
Docs can be found in `docs/`.
Also see `README.md` and `CONTRIBUTING.md` for more information.

## Build/Lint/Test Commands

- Run python code: `uv run path/to/script.py`
- Run all tests: `uv run pytest` or `uv run pytest -m "not skip_ci and no long_running"`
- Run a single test: `uv run pytest tests/path/to/test_file.py::test_function_name -v`
- Format code: `uv run ruff format`
- Lint code: `uv run ruff check --fix`
- Type check: `uv run pyright`

## Code Style Guidelines

- **Formatting**: Follow Google style convention. Use ruff for formatting. Try to follow ruff styles directly when writing code. You can see what rules we have enabled in `pyproject.toml`.
- **Imports**: Use isort order (enforced by ruff). Imports must be at the top of the file, unless there is a very good reason otherwise.
- **Types**: Strict typing is required. A
```

</details>
