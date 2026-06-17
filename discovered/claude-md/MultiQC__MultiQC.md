---
name: MultiQC__MultiQC
source: https://github.com/MultiQC/MultiQC/blob/f2bfddc5c6091569839e27dea228f63b8a8d650c/CLAUDE.md
repo: MultiQC/MultiQC
kind: claude-md
stars: 1461
last_pushed: 2026-06-10T07:10:43Z
license: gpl-3.0
score: 9
domains: [cli-tools, bioinformatics, python]
tags: [architectural-guidance, coding-standards, module-lifecycle]
curated: 2026-06-15
curated_by: config-scout
---

# MultiQC/MultiQC — claude-md

**Why it's worth keeping:** Includes highly actionable logic constraints like 'crash loudly on unexpected data' and provides a clear mental model of the system's data flow; defines mandatory side-effects for modules to ensure architectural consistency.

**Summary:** Provides strict coding standards, architectural patterns, and mandatory module lifecycle rules for adding new features. It emphasizes data integrity by defining specific error-handling behaviors.

**Source credibility:** High; MultiQC is a widely used, highly starred bioinformatics tool with active maintenance.

**Recency:** Current; explicitly mentions Claude Code/claude.ai/code and uses modern Python tooling like ruff and pyproject.toml.

**Source:** [MultiQC/MultiQC/CLAUDE.md](https://github.com/MultiQC/MultiQC/blob/f2bfddc5c6091569839e27dea228f63b8a8d650c/CLAUDE.md) · 1461★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Guidance for Claude Code (claude.ai/code) when working in this repository.

## IMPORTANT

Never push to main. When asked to add a change or open a PR, check the
current branch first; if it's `main`, create a new branch and push to that.

Do NOT create a `Pipfile` — this project uses `pyproject.toml`.

## Style and conventions

- Python 3.9+. Use f-strings and other modern Python 3 syntax. Do not use
  `__future__` imports or `OrderedDict`.
- Double quotes for strings.
- No shebang lines on Python files unless under `scripts/`.
- Type hints are used extensively; mypy enforces.
- Code formatting is enforced with ruff.
- Tests live in `tests/` and use pytest.
- Helpers for distinct parts of the report — one method per section, one
  for parsing, one for general stats — are encouraged. They make
  `__init__` readable as a high-level outline. What to avoid is trivial
  wrappers: a helper that wraps one or two lines, just renames a
  one-liner, or is called once with no logical separation. Ask whether
  the function name is more meaningful than the code it hides; if not,
  inline it.
- Crash loudly on unexpected data. When parsing output from known
  bioinformatics tools, do
```

</details>
