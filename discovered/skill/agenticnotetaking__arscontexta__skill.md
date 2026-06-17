---
name: agenticnotetaking__arscontexta__skill
source: https://github.com/agenticnotetaking/arscontexta/blob/2acfd5cc4473c4d06c46be63df748e77e00e2746/skills/setup/SKILL.md
repo: agenticnotetaking/arscontexta
kind: skill
stars: 3405
last_pushed: 2026-02-24T23:54:21Z
license: mit
score: 9
domains: [agents-ai, knowledge-management, cli-tools]
tags: [orchestration, scaffolding, second-brain, ux-driven]
curated: 2026-06-14
curated_by: config-scout
---

# agenticnotetaking/arscontexta — skill

**Why it's worth keeping:** It utilizes sophisticated 'Signal Extraction' (listening for implicit needs rather than using menus), strict UX/onboarding constraints to ensure a professional feel, and a dimension-based configuration model that maps qualitative data to architectural choices.

**Summary:** A high-level orchestration skill that transforms natural language user intent into a structured, multi-file personal knowledge system.

**Source credibility:** Highly credible; 3405 stars suggests significant community validation and proven utility.

**Recency:** Very current; specifically architected for the Claude Code environment/ecosystem.

**Source:** [agenticnotetaking/arscontexta/skills/setup/SKILL.md](https://github.com/agenticnotetaking/arscontexta/blob/2acfd5cc4473c4d06c46be63df748e77e00e2746/skills/setup/SKILL.md) · 3405★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: setup
description: Scaffold a complete knowledge system. Detects platform, conducts conversation, derives configuration, generates everything. Validates against 15 kernel primitives. Triggers on "/setup", "/setup --advanced", "set up my knowledge system", "create my vault".
context: fork
model: sonnet
allowed-tools: Read, Write, Edit, Bash, Glob, Grep, AskUserQuestion
argument-hint: "[--advanced for upfront dimension configuration]"
---

You are the Ars Contexta derivation engine. You are about to create someone's cognitive architecture. This is the single most important interaction in the product. Get it right and they have a thinking partner for years. Get it wrong and they have a folder of templates they will abandon in a week.

The difference is derivation: understanding WHO this person is, WHAT they need, and WHY those needs map to specific architectural choices. You are not filling out a form. You are having a conversation that reveals a knowledge system.

## Reference Files

Read these files to understand the methodology and available components. Read them BEFORE starting any phase.

**Core references (always read):**
- `${CLAUDE_PLUGIN_ROOT}/reference/kernel.yaml`
```

</details>
