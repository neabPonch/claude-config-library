---
name: caian-org__ansible-stow
source: https://github.com/caian-org/ansible-stow/blob/5087d345b6867078664d9fb6a4d6e70ffe54c68a/CLAUDE.md
repo: caian-org/ansible-stow
kind: claude-md
stars: 39
last_pushed: 2026-05-17T19:32:52Z
license: cc0-1.0
score: 8
domains: [devops, cli-tools, python]
tags: [ansible, automation, module]
curated: 2026-06-15
curated_by: config-scout
---

# caian-org/ansible-stow — claude-md

**Why it's worth keeping:** The 'Architecture' section goes beyond file listings to explain core function behaviors and module states, which provides critical context for LLM reasoning. It also defines explicit quality thresholds like minimum PyLint scores.

**Summary:** A highly actionable guide that combines specific command workflows with an explanation of internal logic and state transitions.

**Source credibility:** A niche DevOps tool with a structured, professional documentation style.

**Recency:** Current; uses modern Python tooling like uv and poe.

**Source:** [caian-org/ansible-stow/CLAUDE.md](https://github.com/caian-org/ansible-stow/blob/5087d345b6867078664d9fb6a4d6e70ffe54c68a/CLAUDE.md) · 39★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

ansible-stow is an Ansible module that wraps GNU Stow for managing symlink farms. It's a single-file module (`stow`) that enables idempotent dotfile/package management in Ansible playbooks.

## Commands

**Install dependencies:**
```bash
uv sync --extra dev
```

**Code quality checks:**
```bash
uv run poe check:style      # Black formatting check (120 char lines)
uv run poe check:lint       # PyLint (must score >= 9)
uv run poe check:security   # Bandit security scan
uv run poe check:deadcode   # Vulture dead code detection
```

**Fix formatting:**
```bash
uv run poe fix:style
```

**Run tests:**
```bash
cd tests && ./test.sh
```

Tests run an Ansible playbook that exercises module states (present, absent, latest, supress) and verifies symlink operations.

## Architecture

- **`stow.py`** - The entire module in one executable Python script (~320 lines). Uses Ansible's `AnsibleModule` base class. Distributed as `stow.py` but invoked as `stow` in playbooks.
- **`tests/`** - Integration tests via `test.sh` that runs `stow.yml` playbook against test
```

</details>
