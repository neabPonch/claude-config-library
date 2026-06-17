---
name: TeamDijon__shopify-rules
source: https://github.com/TeamDijon/shopify-rules/blob/c2a72c58b4888f2f3882dac3da45d96b399cf3c0/CLAUDE.md
repo: TeamDijon/shopify-rules
kind: claude-md
stars: 11
last_pushed: 2026-02-07T21:43:51Z
license: mit
score: 9
domains: [web-frontend, ai-agents, documentation]
tags: [shopify, liquid, meta-rules, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# TeamDijon/shopify-rules — claude-md

**Why it's worth keeping:** It treats the AI as a researcher rather than just a coder by providing procedural 'skills' (slash commands) and a rigorous overlap detection methodology.

**Summary:** A meta-instructional framework for discovering, researching, and codifying Shopify Liquid development rules through specialized AI skills.

**Source credibility:** High structural sophistication suggests it was written by an expert in agentic workflows.

**Recency:** Recent; highly compatible with current Claude Code capabilities.

**Source:** [TeamDijon/shopify-rules/CLAUDE.md](https://github.com/TeamDijon/shopify-rules/blob/c2a72c58b4888f2f3882dac3da45d96b399cf3c0/CLAUDE.md) · 11★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# shopify-rules

A collection of AI-consumable rules for Shopify Liquid theme development, plus skills to create more.

## Project structure

- `rules/INDEX.md` -- master index of all rules
- `rules/BACKLOG.md` -- pending topics discovered but not yet written as rules
- `rules/<category>/` -- rule files organized by category (folders created as needed)
- `shopify-themes/` -- optional user-supplied Shopify themes for research (gitignored)

## Available skills

- `/discover-rule-topics <optional focus>` -- mine themes for patterns, enrich the backlog
- `/research-shopify-rule <topic>` -- deep cross-theme research, produce a thorough rule (5 phases)
- `/quick-rule <topic>` -- fast rule creation from official docs (3 phases)

## Overlap detection

Before creating a rule, check for overlap at three levels:

1. `existing-coverage.md` (in skill references) -- static summary of Horizon's 43 cursor rules
2. `rules/INDEX.md` -- rules already written in this repo
3. `shopify-themes/horizon/.cursor/rules/` -- live scan if Horizon theme is present

## Guidelines

- Rules are standalone markdown files. Do not reference project-specific paths within rule content.
- Never invent Liquid filters, ta
```

</details>
