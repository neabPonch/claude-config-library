---
name: samcab28__Repo-Inspector
source: https://github.com/samcab28/Repo-Inspector/blob/2efadd67df627968f84b636aa5f1eeab8d817238/Claude.md
repo: samcab28/Repo-Inspector
kind: claude-md
stars: 0
last_pushed: 2026-03-15T21:40:18Z
license: other
score: 9
domains: [cli-tools, python, static-analysis]
tags: [architecture-centric, data-structures, rule-based]
curated: 2026-06-14
curated_by: config-scout
---

# samcab28/Repo-Inspector — claude-md

**Why it's worth keeping:** The 'Architecture Rules' section enforces structural integrity, while the 'Key Data Structures' section provides necessary type-awareness for generating new logic. The inclusion of a specific 'Adding a new analyzer' checklist is a perfect template for guiding agentic workflows.

**Summary:** This file provides an exhaustive blueprint of the project by defining not just structure, but strict architectural constraints and data schemas. It transforms an AI from a generic coder into a domain-aware contributor.

**Source credibility:** Low social proof (0 stars), but demonstrates high technical maturity through its rigorous documentation of rules and data types.

**Recency:** Highly current; provides the exact depth of structural detail required by modern coding agents like Claude Code.

**Source:** [samcab28/Repo-Inspector/Claude.md](https://github.com/samcab28/Repo-Inspector/blob/2efadd67df627968f84b636aa5f1eeab8d817238/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Repo Inspector

## Project Overview

Repo Inspector is an open-source Python CLI tool that performs static analysis on local code repositories.
It runs fully offline, requires no external APIs, and is distributed as a pip package.

The tool analyzes Python projects using AST parsing, dependency graph construction,
and structural heuristics to surface code quality metrics, architectural issues, and
technical debt indicators.

**Status:** fully implemented. All analyzers, CLI commands, tests (211), and packaging are complete.

---

## Tech Stack

- Python 3.11+
- Typer (CLI framework)
- Rich (terminal output formatting)
- Radon (cyclomatic complexity calculation)
- NetworkX (dependency graph construction and cycle detection)
- Pathspec (gitignore-aware file traversal)
- Hatch (build and packaging)
- pytest (test suite)

---

## Project Structure

```
repo_inspector/
    cli.py                      # Typer CLI entrypoint, all command definitions
    scanner/
        project_scanner.py      # File traversal, gitignore handling, ProjectIndex builder
    analysis/
        complexity.py           # Cyclomatic complexity per function, large file detection
        coupling.py
```

</details>
