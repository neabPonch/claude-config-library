---
name: hericlibong__Observatoire_racism
source: https://github.com/hericlibong/Observatoire_racism/blob/67a84f2956816fd69702be86c17ff29aec39c444/CLAUDE.md
repo: hericlibong/Observatoire_racism
kind: claude-md
stars: 0
last_pushed: 2026-04-22T20:31:18Z
license: unknown
score: 9
domains: [data-pipeline, python, ai-agents]
tags: [architecture-mapping, business-logic, constraints]
curated: 2026-06-15
curated_by: config-scout
---

# hericlibong/Observatoire_racism — claude-md

**Why it's worth keeping:** The 'Contract invariants' section provides crucial domain constraints that prevent AI from breaking logic; the architecture mapping offers high-density structural context.

**Summary:** Defines a rigorous technical and business framework for a data pipeline, including explicit architectural layers and command-line workflows.

**Source credibility:** Low social proof (0 stars), but content quality suggests a professional/academic data engineering project.

**Recency:** Current, utilizing modern Python 3.12 and contemporary tooling like Ruff and Mypy.

**Source:** [hericlibong/Observatoire_racism/CLAUDE.md](https://github.com/hericlibong/Observatoire_racism/blob/67a84f2956816fd69702be86c17ff29aec39c444/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Python 3.12+ data pipeline for analyzing French parliamentary debates (Assemblée nationale, Syceron XML corpus). Detects hate speech, racism, xenophobia, discrimination, and problematic group-targeting signals. Contextualizes via Mistral LLM.

Scope is strictly limited to discriminatory signals. This project must not become a general political-tension or civic-climate observatory.

Key reference docs:
- `docs/assemblee_roadmap.md` — planning source of truth
- `docs/assemblee_contextualization_contract_v2.md` — V2 contract reference
- `docs/audit_architecture.md` — architecture audit and Phase G refactoring roadmap

## Commands

```bash
# Install (editable, with dev deps)
python -m pip install -e '.[dev]'

# Test
python -m pytest tests/ -v

# Run a single test file
python -m pytest tests/assemblee_contextualization/test_review_engine.py -v

# Lint (check)
python -m ruff check src tests

# Format
python -m ruff format src tests

# Type check
python -m mypy src tests
```

## Architecture

**Data flow:**
```
ZIP archive → source_acquisition → XML files (data/
```

</details>
