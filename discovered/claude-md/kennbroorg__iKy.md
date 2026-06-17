---
name: kennbroorg__iKy
source: https://github.com/kennbroorg/iKy/blob/2abf97d8736dfa1503a6706d56082c94e07f1a23/CLAUDE.md
repo: kennbroorg/iKy
kind: claude-md
stars: 960
last_pushed: 2026-06-14T14:15:02Z
license: gpl-3.0
score: 8
domains: [backend-api, security, python]
tags: [ruff, just-commands, flask]
curated: 2026-06-15
curated_by: config-scout
---

# kennbroorg/iKy — claude-md

**Why it's worth keeping:** It provides highly specific linting rule sets (e.g., E, F, W) and explicit command mappings for toolchains, which prevents the AI from hallucinating its own build steps.

**Summary:** Defines project structure, rigorous Python linting rules using Ruff, and standard development workflows via 'just' commands.

**Source credibility:** High; a highly-starred OSINT tool with recent maintenance activity.

**Recency:** Current; specifies modern Python 3.12 idioms and up-to-date linting standards.

**Source:** [kennbroorg/iKy/CLAUDE.md](https://github.com/kennbroorg/iKy/blob/2abf97d8736dfa1503a6706d56082c94e07f1a23/CLAUDE.md) · 960★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# iKy - OSINT Tool

## Project Structure

- `backend/` — Python 3.12 Flask + Celery backend
- `frontend/` — Angular frontend
- `install/docker/` — Dockerfiles and compose config

## Coding Style

All Python code MUST comply with the project's `ruff.toml` configuration:

- **Formatter**: ruff format (black-compatible), line-length 88, target py312
- **Linter rules**: E, F, W (pycodestyle/pyflakes), I (isort), B (bugbear), UP (pyupgrade), SIM (simplify), C4 (comprehensions), A (builtins), RUF (ruff-specific)
- **Ignored**: E203 (black-compatible whitespace), E501 (line length handled by formatter)
- **Tests**: S101 (assert usage) is allowed in `**/tests/**`

When writing or modifying Python code:

1. Use modern Python 3.12 idioms (f-strings, `|` union types, `match`, etc.)
2. Keep lines at 88 chars max
3. Sort imports with isort style (stdlib, third-party, local — separated by blank lines)
4. Prefer list/dict/set comprehensions over map/filter
5. Avoid shadowing Python builtins (rule A)
6. Use `pathlib.Path` over `os.path` where practical

## Dev Workflow

- `just setup` — create `.venv/` with pre-commit and ruff (pinned to match pre-commit config)
- `just lint` / `just fmt` — check
```

</details>
