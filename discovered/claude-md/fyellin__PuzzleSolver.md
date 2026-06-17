---
name: fyellin__PuzzleSolver
source: https://github.com/fyellin/PuzzleSolver/blob/12c452fa06a968129964c2711e345fc9e761b04f/CLAUDE.md
repo: fyellin/PuzzleSolver
kind: claude-md
stars: 0
last_pushed: 2026-04-19T01:56:10Z
license: unknown
score: 8
domains: [python, software-engineering]
tags: [style-guide, typing, ruff, modern-python]
curated: 2026-06-15
curated_by: config-scout
---

# fyellin/PuzzleSolver — claude-md

**Why it's worth keeping:** It uses powerful 'negative constraints' to prevent unwanted ruff formatting and provides detailed instructions for structural subtyping via Protocols.

**Summary:** A highly specific Python style guide that mandates modern typing standards and explicitly restricts automated formatting to maintain code density.

**Source credibility:** Low social proof (0 stars), but the content demonstrates high-level Python expertise/modernity.

**Recency:** Very current, utilizing modern PEPs like PEP 695 for generics.

**Source:** [fyellin/PuzzleSolver/CLAUDE.md](https://github.com/fyellin/PuzzleSolver/blob/12c452fa06a968129964c2711e345fc9e761b04f/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Python Preliminary Rule

Match the style of `solver/` unless a file already follows a different local convention.

## Core expectations

- Prefer clear, readable code over clever shortcuts.
- Keep functions focused and small when practical.
- Add type hints for new or changed public functions.
- Handle errors explicitly; avoid silent failures.
- Automatically update the imports in the style expected by ruff. Delete any unused imports as necessary.
- Do NOT format using "ruff format". I do not like each argument of a function and each element of a list on a separate line. I only want the imports to be in ruff format.

## Style reference: `solver/` package

Follow this when editing Python in this repo:

- **Imports**: Standard library first, then a blank line, then project imports (`from .module import ...`). Keep imports sorted and grouped the way ruff expects; do not run full-file `ruff format` on argument lists or collections.
- **Typing**: Use modern annotations throughout (`list[str]`, `X | None`, `Sequence[T]` from `collections.abc`). Use `type Name = ...` for common dict/alias types. Prefer `collections.abc` (`Sequence`, `Mapping`, `Callable`, `Iterable`) over concrete `list
```

</details>
