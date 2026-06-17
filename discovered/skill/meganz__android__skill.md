---
name: meganz__android__skill
source: https://github.com/meganz/android/blob/b0650d7ef285ee372927e365feebc440a908b8e9/.claude/skills/mega-figma-to-compose/SKILL.md
repo: meganz/android
kind: skill
stars: 1848
last_pushed: 2026-06-12T11:24:05Z
license: other
score: 9
domains: [android, mobile-app-dev, ui-ux]
tags: [figma, compose, design-system, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# meganz/android — skill

**Why it's worth keeping:** It demonstrates elite instruction engineering: using visual workflows (dot diagrams), 'non-negotiable' constraint lists, and proactive error mitigation through 'Red flags' and 'Common mistakes' sections. The pattern of forcing the agent to 'grep before creating' is a highly transferable technique for large codebases.

**Summary:** A rigorous skill for translating Figma designs into a specific Android design system via Jetpack Compose. It enforces strict architectural constraints and includes a mandatory multi-step verification workflow.

**Source credibility:** High; derived from a major production Android repository with significant star count.

**Recency:** Current; aligns perfectly with modern Claude Code skill/agent patterns and mobile development workflows.

**Source:** [meganz/android/.claude/skills/mega-figma-to-compose/SKILL.md](https://github.com/meganz/android/blob/b0650d7ef285ee372927e365feebc440a908b8e9/.claude/skills/mega-figma-to-compose/SKILL.md) · 1848★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: figma-to-mega-compose
description: >
  Use when given a Figma URL or node and asked to translate it into MEGA Android
  Jetpack Compose code, before writing any UI code. Triggers include "implement
  this Figma", "build this design", "translate Figma to Compose", or any message
  containing a figma.com link plus a request for Compose / Android UI. Encodes
  MEGA's Core-UI component mapping, design-token rules, and the rule that
  existing screens MUST be located before any new code is written.
triggers:
  - /figma-to-mega-compose
  - implement this Figma
  - build this design in Compose
  - translate Figma to Compose
  - figma.com/design
  - figma.com/make
---

# Figma → MEGA Compose Skill

Translate Figma designs into MEGA Android Jetpack Compose code, reusing Core-UI components and project conventions. Composes on top of `figma:figma-implement-design` (generic) by adding MEGA-specific knowledge.

## When to use

- User pastes a `figma.com/design/...` or `figma.com/make/...` link and asks for Compose / Android code.
- User says "implement / build / translate this Figma in Compose".

## When NOT to use

- Editing an existing Compose UI without a Figma source → just edit t
```

</details>
