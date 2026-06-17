---
name: OpenMDAO__OpenMDAO
source: https://github.com/OpenMDAO/OpenMDAO/blob/6d45412a0ee6ee98d1b0a097b50166588bfe4a64/CLAUDE.md
repo: OpenMDAO/OpenMDAO
kind: claude-md
stars: 740
last_pushed: 2026-06-03T17:54:15Z
license: other
score: 7
domains: [scientific-computing, python]
tags: [pixi, testing-workflow, linting]
curated: 2026-06-15
curated_by: config-scout
---

# OpenMDAO/OpenMDAO — claude-md

**Why it's worth keeping:** It provides specific commands for scoped test execution to save time/resources and sets clear boundaries on how the agent should handle git interactions.

**Summary:** Defines the development environment via pixi and specifies strict code style and testing procedures.

**Source credibility:** High; OpenMDAO is a major, highly-starred scientific computing repository.

**Recency:** Current; utilizes modern toolchains like pixi and ruff.

**Source:** [OpenMDAO/OpenMDAO/CLAUDE.md](https://github.com/OpenMDAO/OpenMDAO/blob/6d45412a0ee6ee98d1b0a097b50166588bfe4a64/CLAUDE.md) · 740★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project

OpenMDAO provides analysis and optimization of multidisciplinary systems using the modular approach to unified derivatives.

# Development Guidelines

- Use the "dev" environment in the pixi.toml file in the root of this project.

- Do not invoke git commands, but suggest a commit message.

# Code Style

- Use single quotes, except to define docstrings. When nesting quotes, use double quotes for the outer string.

- Documentation is in the numpy doc style.

- Do not use emojis.

# Validation

- Generated code should pass `ruff check`. Rules for ruff are established in pyproject.toml.

- Use `pixi run test <path>` to invoke tests in the relevant scope. Only run `pixi run test` if the user asks for the full test suite.
```

</details>
