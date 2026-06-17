---
name: tradermonty__claude-trading-skills
source: https://github.com/tradermonty/claude-trading-skills/blob/b5566100dfad877f81fbad172293e2195f451919/CLAUDE.md
repo: tradermonty/claude-trading-skills
kind: claude-md
stars: 1914
last_pushed: 2026-06-14T14:29:10Z
license: mit
score: 9
domains: [agents-ai, fintech, cli-tools]
tags: [skill-architecture, agentic-workflows, automation]
curated: 2026-06-15
curated_by: config-scout
---

# tradermonty/claude-trading-skills — claude-md

**Why it's worth keeping:** Provides high-density structural patterns and explicit CLI workflows that allow Claude to act as a platform maintainer rather than just a coder.

**Summary:** Defines a sophisticated framework for creating 'skills' by strictly separating domain knowledge (markdown) from executable logic (scripts).

**Source credibility:** Highly credible with ~1.9k stars and extremely active maintenance.

**Recency:** Very current; explicitly designed for the Claude Code environment.

**Source:** [tradermonty/claude-trading-skills/CLAUDE.md](https://github.com/tradermonty/claude-trading-skills/blob/b5566100dfad877f81fbad172293e2195f451919/CLAUDE.md) · 1914★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This repository contains Claude Skills for equity investors and traders. Each skill packages domain-specific prompts, knowledge bases, and helper scripts to assist with market analysis, technical charting, economic calendar monitoring, and trading strategy development. Skills are designed to work in both Claude's web app and Claude Code environments.

⚠️ **Important:** Some skills require paid API subscriptions (FMP API and/or FINVIZ Elite) to function. See the [API Key Management](#api-key-management) section for detailed requirements by skill.

## Repository Architecture

### Skill Structure

Each skill follows a standardized directory structure:

```
<skill-name>/
├── SKILL.md              # Required: Skill definition with YAML frontmatter
├── references/           # Knowledge bases loaded into Claude's context
├── scripts/             # Executable Python scripts (not auto-loaded)
└── assets/              # Templates and resources for output generation
```

**SKILL.md Format:**
- YAML frontmatter with `name` and `description` fields
- `name`
```

</details>
