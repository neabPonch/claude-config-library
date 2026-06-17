---
name: yusufkaraaslan__Skill_Seekers
source: https://github.com/yusufkaraaslan/Skill_Seekers/blob/61911d0efa72ae506acf7242f4775a9ddc6a3466/CLAUDE.md
repo: yusufkaraaslan/Skill_Seekers
kind: claude-md
stars: 14077
last_pushed: 2026-06-11T21:20:13Z
license: mit
score: 9
domains: [cli-tools, agents-ai, python]
tags: [architecture-documentation, test-optimization, workflow-guidance]
curated: 2026-06-15
curated_by: config-scout
---

# yusufkaraaslan/Skill_Seekers — claude-md

**Why it's worth keeping:** The 'Essential Commands' section includes specific patterns to skip slow tests for faster iteration, while the detailed 'Scan command' documentation prevents the AI from making incorrect assumptions about file handling or state changes.

**Summary:** A high-density technical guide that provides precise CLI commands, test execution shortcuts, and deep architectural logic for an AI-driven discovery tool.

**Source credibility:** High; 14k stars indicates a highly popular and well-maintained open-source project.

**Recency:** Current; incorporates modern Python tooling (uv, ruff) and reflects recent architectural updates.

**Source:** [yusufkaraaslan/Skill_Seekers/CLAUDE.md](https://github.com/yusufkaraaslan/Skill_Seekers/blob/61911d0efa72ae506acf7242f4775a9ddc6a3466/CLAUDE.md) · 14077★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Skill Seekers** converts documentation from 18 source types into production-ready formats for 21+ AI platforms (LLM platforms, RAG frameworks, vector databases, AI coding assistants). Published on PyPI as `skill-seekers`.

**Version:** 3.7.0 | **Python:** 3.10+ | **Website:** https://skillseekersweb.com/

**Architecture:** See `docs/UML_ARCHITECTURE.md` for UML diagrams and module overview. StarUML project at `docs/UML/skill_seekers.mdj`. Refactor state/history: `docs/UNIFICATION_PLAN.md` (Grand Unification — all 5 phases done; remaining cosmetic items listed there).

## Essential Commands

```bash
# REQUIRED before running tests or CLI (src/ layout)
pip install -e .

# Run all tests (NEVER skip - all must pass before commits)
pytest tests/ -v

# Fast iteration (skip slow MCP tests ~20min)
pytest tests/ --ignore=tests/test_mcp_fastmcp.py --ignore=tests/test_mcp_server.py --ignore=tests/test_install_skill_e2e.py -q

# Single test
pytest tests/test_scraper_features.py::test_detect_language -vv -s

# Code quality (must pass before push - matches C
```

</details>
