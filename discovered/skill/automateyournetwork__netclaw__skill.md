---
name: automateyournetwork__netclaw__skill
source: https://github.com/automateyournetwork/netclaw/blob/b7a930130210999eb10865af60f8cdf6ed473a8b/workspace/skills/aap-lint/SKILL.md
repo: automateyournetwork/netclaw
kind: skill
stars: 556
last_pushed: 2026-06-15T13:17:21Z
license: apache-2.0
score: 8
domains: [devops, infrastructure-as-code, cli-tools]
tags: [ansible, linting, automation]
curated: 2026-06-16
curated_by: config-scout
---

# automateyournetwork/netclaw — skill

**Why it's worth keeping:** It uses structured 'Workflows' to teach the agent how to sequence tools, and includes 'Important Rules' that provide decision logic (e.g., choosing profiles based on environment).

**Summary:** Provides a specialized capability for validating Ansible playbooks and roles using ansible-lint via an MCP server.

**Source credibility:** High; part of a well-regarded network automation repository with recent activity.

**Recency:** 

**Source:** [automateyournetwork/netclaw/workspace/skills/aap-lint/SKILL.md](https://github.com/automateyournetwork/netclaw/blob/b7a930130210999eb10865af60f8cdf6ed473a8b/workspace/skills/aap-lint/SKILL.md) · 556★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: aap-lint
description: "ansible-lint playbook and role validation — syntax checking, best practice enforcement, project-wide analysis, rule filtering. Use when validating Ansible playbooks, checking code quality, or enforcing automation best practices before deployment."
version: 1.0.0
license: Apache-2.0
tags: [ansible, lint, quality, validation, best-practices, playbook]
metadata:
  { "openclaw": { "requires": { "bins": ["python3", "ansible-lint"] } } }
---

# Ansible Lint Operations

## MCP Server

- **Repository**: [sibilleb/AAP-Enterprise-MCP-Server](https://github.com/sibilleb/AAP-Enterprise-MCP-Server)
- **Transport**: stdio (Python via `uv run ansible-lint.py`)
- **Install**: `git clone` + `uv sync` (or `pip install -e .`)
- **Requires**: `ansible-lint` installed

## Available Tools (9)

| Tool | What It Does |
|------|-------------|
| `lint_playbook` | Lint playbook content with configurable profiles and output formats |
| `lint_file` | Lint a specific Ansible file at a given path |
| `lint_role` | Comprehensive linting of an Ansible role directory |
| `list_rules` | Display available ansible-lint rules with optional tag filtering |
| `list_tags` | Show all tags f
```

</details>
