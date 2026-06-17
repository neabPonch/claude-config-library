---
name: emanueleielo__ciana-parrot__add-skill
source: https://github.com/emanueleielo/ciana-parrot/blob/d289c767a51b35cba43b003bd12ac2f1aa5b7471/docs/guides/add-skill.md
repo: emanueleielo/ciana-parrot
kind: skill
stars: 75
last_pushed: 2026-04-20T14:45:00Z
license: mit
score: 8
domains: [agents-ai, backend-api]
tags: [modular-architecture, auto-discovery, tool-registration]
curated: 2026-06-15
curated_by: config-scout
---

# emanueleielo/ciana-parrot — skill

**Why it's worth keeping:** It implements 'pre-flight' dependency gating via `requires_env` and `requires_bridge`, preventing the agent from attempting to use tools whose prerequisites are not met.

**Summary:** A modular architecture for agent skills that uses auto-discovered directories containing both metadata (SKILL.md) and implementation (skill.py).

**Source credibility:** Decent; a growing open-source project with active maintenance and high-quality documentation.

**Recency:** Highly current, utilizing modern LangChain tool decorators.

**Source:** [emanueleielo/ciana-parrot/docs/guides/add-skill.md](https://github.com/emanueleielo/ciana-parrot/blob/d289c767a51b35cba43b003bd12ac2f1aa5b7471/docs/guides/add-skill.md) · 75★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
title: Add a Skill
---

# Add a Skill

This guide shows you how to create a skill -- a self-contained package of tools that the agent discovers automatically at startup.

---

## Introduction

Skills are the easiest way to extend CianaParrot. A skill is a folder inside `workspace/skills/` containing two files:

- **`SKILL.md`** -- a markdown file with YAML frontmatter that describes the skill to the agent
- **`skill.py`** -- a Python file with `@tool`-decorated functions that auto-register as agent tools

DeepAgents discovers skills at startup by scanning the skills directory. The agent receives the skill description as context and can call the skill's tools during conversations.

---

## Prerequisites

- A working CianaParrot installation ([Installation Guide](../getting-started/installation.md))
- The skills system enabled in config (default: `skills.enabled: true`)
- Basic familiarity with LangChain's `@tool` decorator

---

## Step 1: Create the Skill Directory

```bash
mkdir -p workspace/skills/my-skill
```

!!! note "Path inside Docker"
    The `workspace/` directory is mounted into the container at `/app/workspace`. The agent sees skills at the virtual path `skills/my-sk
```

</details>
