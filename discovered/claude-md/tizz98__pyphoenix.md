---
name: tizz98__pyphoenix
source: https://github.com/tizz98/pyphoenix/blob/385dcdba410af32695ccf611d9cf3f2815995184/CLAUDE.md
repo: tizz98/pyphoenix
kind: claude-md
stars: 0
last_pushed: 2025-08-14T15:06:31Z
license: mit
score: 8
domains: [backend, distributed-systems, python]
tags: [architecture, poetry, asyncio]
curated: 2026-06-16
curated_by: config-scout
---

# tizz98/pyphoenix — claude-md

**Why it's worth keeping:** The 'Core Architecture Concepts' and 'Process Model' sections provide vital mental models that prevent an LLM from suggesting implementations that violate the project's structural goals.

**Summary:** Provides comprehensive architectural context for a distributed real-time communication library, bridging the gap between low-level commands and high-level design intent.

**Source credibility:** Low visibility (0 stars) but demonstrates high-quality documentation practices for a new project.

**Recency:** Highly current, targeting Python 3.13 and modern developer tooling like Ruff and Poetry.

**Source:** [tizz98/pyphoenix/CLAUDE.md](https://github.com/tizz98/pyphoenix/blob/385dcdba410af32695ccf611d9cf3f2815995184/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

This project uses Poetry for dependency management and packaging:

- **Install dependencies**: `poetry install`
- **Run tests**: `poetry run pytest`
- **Code formatting**: `poetry run ruff format .`
- **Code linting**: `poetry run ruff check .`
- **Fix linting issues**: `poetry run ruff check --fix .`
- **Build package**: `poetry build`
- **Run Python scripts**: `poetry run python <script.py>`
- **Add dependencies**: `poetry add <package>`
- **Add dev dependencies**: `poetry add --group dev <package>`

## Project Architecture

PyPhoenix is a Python library designed to bring Elixir Phoenix-style real-time communication channels to Python applications. The project is in early development stage.

### Core Architecture Concepts

The library is designed around several key abstractions:

1. **Channels**: Primary abstraction for real-time communication representing conversations on specific topics
2. **Topics**: Hierarchical string identifiers for message routing (e.g., `"room:123"`, `"user:456:notifications"`)
3. **Presence**: Distributed presence
```

</details>
