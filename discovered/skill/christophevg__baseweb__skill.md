---
name: christophevg__baseweb__skill
source: https://github.com/christophevg/baseweb/blob/ab13ba40aa114752324ddb300c138ee45a354210/skills/create/skill.md
repo: christophevg/baseweb
kind: skill
stars: 1
last_pushed: 2026-06-07T14:06:10Z
license: mit
score: 8
domains: [web-development, python, scaffolding]
tags: [baseweb, project-scaffolding, vue, uv]
curated: 2026-06-16
curated_by: config-scout
---

# christophevg/baseweb — skill

**Why it's worth keeping:** It utilizes high-fidelity file templates (including Makefile and pyproject.toml) and a clear decision tree to move the agent from project intent to a fully functional, runnable environment.

**Summary:** A specialized scaffolding skill that provides a comprehensive blueprint for creating Baseweb applications across various complexity levels.

**Source credibility:** Low visibility; appears to be a niche or personal framework/template library.

**Recency:** Current; uses modern tooling like `uv` and Python 3.12.

**Source:** [christophevg/baseweb/skills/create/skill.md](https://github.com/christophevg/baseweb/blob/ab13ba40aa114752324ddb300c138ee45a354210/skills/create/skill.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: baseweb-create
description: Create new baseweb applications with guided setup
triggers:
  - when asked to create a new baseweb project
  - when setting up a new web application
  - when starting a new baseweb-based project
---

# Baseweb Create Skill

Guide users through creating new baseweb applications with appropriate structure and configuration.

## Overview

This skill helps create new baseweb projects by:

1. Asking clarifying questions about project needs
2. Generating appropriate project structure
3. Creating initial configuration files
4. Setting up development environment

## When to Use

- Creating a new baseweb project
- Starting a new web application with baseweb
- Setting up a project template

## Project Flavors

Baseweb supports different project types:

| Flavor | Description | Use Case |
|--------|-------------|----------|
| **minimal** | Basic setup with one page | Simple apps, learning |
| **standard** | REST API + pages | Typical web applications |
| **full** | REST API + WebSocket + Auth | Complex interactive apps |
| **pwa** | Progressive Web App | Installable web apps |
| **api-only** | REST API without UI | Backend services |

## Setup Questions
```

</details>
