---
name: palkan__action_policy__skill
source: https://github.com/palkan/action_policy/blob/3dc0928eff6891df295fe049f119ac49bce95742/tutorial/.claude/skills/tutorial-lesson-config/SKILL.md
repo: palkan/action_policy
kind: skill
stars: 1563
last_pushed: 2026-03-25T10:05:47Z
license: mit
score: 9
domains: [web-development, cli-tools, configuration]
tags: [yaml, inheritance, rails, config]
curated: 2026-06-15
curated_by: config-scout
---

# palkan/action_policy — skill

**Why it's worth keeping:** It utilizes highly effective 'WRONG vs CORRECT' patterns to explain complex array-replacement logic in inheritance, preventing common configuration errors.

**Summary:** A technical specification for configuring lesson frontmatter, detailing inheritance cascades and environment settings for terminals, editors, and previews.

**Source credibility:** High-quality technical documentation; content is extremely structured despite the repo description mismatch.

**Recency:** Current; uses modern Rails and WebContainer development patterns.

**Source:** [palkan/action_policy/tutorial/.claude/skills/tutorial-lesson-config/SKILL.md](https://github.com/palkan/action_policy/blob/3dc0928eff6891df295fe049f119ac49bce95742/tutorial/.claude/skills/tutorial-lesson-config/SKILL.md) · 1563★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: tutorial-lesson-config
description: |
  Use this skill whenever configuring lesson frontmatter or checking inheritance rules.
  Trigger on: 'frontmatter', 'prepareCommands', 'mainCommand', 'editor config', 'terminal
  config', 'preview config', 'configuration inheritance', 'focus file', 'i18n', 'allowEdits',
  'previews', 'autoReload', 'scope', 'defaults', 'what inherits', 'does X inherit',
  'invalid combination', 'constraint', or any YAML frontmatter question — even without
  mentioning configuration. Authoritative reference for all frontmatter options, inheritance
  rules, defaults, and invalid-combination constraints with Rails-specific patterns. Do NOT
  guess frontmatter without this skill. Do NOT use for content hierarchy
  (use tutorial-content-structure) or file organization (use rails-file-management).
---

# Tutorial Lesson Configuration

Complete reference for configuring lessons, with Rails-specific defaults and patterns.

## Configuration Cascade

Configuration **inherits downward**: Tutorial > Part > Chapter > Lesson. Set shared defaults at the tutorial level; override per-lesson as needed.

```
meta.md (type: tutorial)     ← base defaults for all lessons
```

</details>
