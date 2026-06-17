---
name: trustedsec__hate_crack
source: https://github.com/trustedsec/hate_crack/blob/b0e6cc31598a57d3029bef93ea8e8f5e457eca0a/CLAUDE.md
repo: trustedsec/hate_crack
kind: claude-md
stars: 1834
last_pushed: 2026-05-28T16:10:19Z
license: unknown
score: 9
domains: [cli-tools, security, python]
tags: [architecture-patterns, workflow-rules, checklist, git-worktrees]
curated: 2026-06-15
curated_by: config-scout
---

# trustedsec/hate_crack — claude-md

**Why it's worth keeping:** It includes highly actionable checklists for feature addition and an essential workflow policy to prevent filesystem conflicts during parallel agent execution.

**Summary:** This file provides exhaustive architectural wiring instructions, including a multi-file 'Three-Layer Attack Pattern' checklist and mandatory git worktree usage.

**Source credibility:** High; comes from a widely used security automation tool with significant GitHub traction.

**Recency:** Modern; utilizes contemporary tooling like `uv` and follows current development best practices.

**Source:** [trustedsec/hate_crack/CLAUDE.md](https://github.com/trustedsec/hate_crack/blob/b0e6cc31598a57d3029bef93ea8e8f5e457eca0a/CLAUDE.md) · 1834★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

hate_crack is a menu-driven Python wrapper for hashcat that automates password cracking methodologies. It provides 16 attack modes, API integrations (Hashview, Weakpass, Hashmob), and utilities for wordlist/rule management.

## Commands

```bash
# Install (builds submodules, vendors assets, installs via uv)
make install

# Dev install (editable, with dev deps)
make dev-install

# Run tests (requires HATE_CRACK_SKIP_INIT=1 in worktrees without hashcat-utils)
HATE_CRACK_SKIP_INIT=1 uv run pytest -v

# Run a single test file
HATE_CRACK_SKIP_INIT=1 uv run pytest tests/test_ui_menu_options.py -v

# Lint
uv run ruff check hate_crack
uv run ty check hate_crack

# Both lint checks
make lint

# Format
uv run ruff format hate_crack

# Coverage
make coverage
```

**Test environment variables**: `HATE_CRACK_SKIP_INIT=1` skips binary/config validation (essential for worktrees without hashcat-utils). `HASHMOB_TEST_REAL=1`, `HASHVIEW_TEST_REAL=1`, `WEAKPASS_TEST_REAL=1` enable live API tests.

## Git Hooks

Git hooks are managed by [prek](https://github.com/j178/pr
```

</details>
