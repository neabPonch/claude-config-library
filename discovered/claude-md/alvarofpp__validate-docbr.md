---
name: alvarofpp__validate-docbr
source: https://github.com/alvarofpp/validate-docbr/blob/361a4e8846268bbe140759b3a495fb6e71e398b1/CLAUDE.md
repo: alvarofpp/validate-docbr
kind: claude-md
stars: 482
last_pushed: 2026-04-04T17:51:24Z
license: mit
score: 9
domains: [cli-tools, python]
tags: [architecture-patterns, workflow-automation, tooling]
curated: 2026-06-15
curated_by: config-scout
---

# alvarofpp/validate-docbr — claude-md

**Why it's worth keeping:** The 'Adding a New Document' workflow provides an actionable recipe for LLMs to extend the codebase without hallucinating implementations; the explicit command list minimizes tool-usage errors.

**Summary:** A highly structured guide that details specific tooling (uv, Task), architectural patterns, and exact commands for testing and linting.

**Source credibility:** High; backed by a popular, well-maintained Python package with 482 stars.

**Recency:** Current; uses modern tools like uv and follows recent Python type hinting standards.

**Source:** [alvarofpp/validate-docbr/CLAUDE.md](https://github.com/alvarofpp/validate-docbr/blob/361a4e8846268bbe140759b3a495fb6e71e398b1/CLAUDE.md) · 482★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code)
when working with code in this repository.

## Project Overview

**validate-docbr** is a Python package for validating and
generating Brazilian documents (CPF, CNPJ, CNH, CNS, PIS,
Título Eleitoral, RENAVAM, Certidão). Published on PyPI as
`validate-docbr`, version **2.0.0**.

## Language Conventions

- **Code** (class names, method names, variables): **English**
- **Comments, docstrings, docs, commits, issues**: **pt-BR**
- **Claude files** (CLAUDE.md, agents, commands): **English**

## Tooling

- **Package manager**: [uv](https://docs.astral.sh/uv/)
  (`pyproject.toml` + `uv.lock`)
- **Type checker**: [ty](https://docs.astral.sh/ty/)
- **Task runner**: [Task](https://taskfile.dev/)
  (`Taskfile.yml`)
- **Tests**: pytest 9.0.2 + pytest-cov 7.1.0
- **Python**: >= 3.10 (tested 3.10–3.14)

## Commands

```bash
task build            # Build Docker image (installs git hooks)
task test             # Run all tests with pytest
task test-coverage    # Run tests with coverage (threshold 98%)
task type-check       # Run ty type checker
task lint             # Run all linters
task lint-fix         # Auto-fix Python lint
```

</details>
