---
name: metabase__metabase__skill
source: https://github.com/metabase/metabase/blob/f6353738307a24b767f2574f9b1fac3abe663750/.claude/skills/emotion-migrate/SKILL.md
repo: metabase/metabase
kind: skill
stars: 47681
last_pushed: 2026-06-15T05:27:10Z
license: other
score: 9
domains: [web-frontend, refactoring]
tags: [migration, mantine, react, styling]
curated: 2026-06-15
curated_by: config-scout
---

# metabase/metabase — skill

**Why it's worth keeping:** It provides a 'Decision Gate' logic that prevents LLM-driven refactor bloat and includes explicit property mapping tables (e.g., color -> c) for high accuracy. The strict naming/import conventions ensure the resulting code matches professional codebase standards.

**Summary:** A high-precision migration skill for converting Emotion styled-components to Mantine components and CSS modules. It uses structured decision gates to enforce design system consistency.

**Source credibility:** High; derived from Metabase, a large-scale, highly-starred open source project.

**Recency:** Current; addresses modern React design system migration patterns.

**Source:** [metabase/metabase/.claude/skills/emotion-migrate/SKILL.md](https://github.com/metabase/metabase/blob/f6353738307a24b767f2574f9b1fac3abe663750/.claude/skills/emotion-migrate/SKILL.md) · 47681★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: emotion-migrate
description: Migrate Emotion styled-components to Mantine components with style props and CSS modules. Use when converting .styled.tsx files or removing @emotion imports from components.
---

# Emotion → Mantine + CSS Modules Migration Skill

Migrate Emotion styled-components (`@emotion/styled`, `@emotion/react`) to Mantine layout components with style props and CSS modules. The goal is zero Emotion imports, zero inline styles, and maximum use of design system tokens.

## Priority Order (Strict)

1. **Mantine components + style props** — `Box`, `Flex`, `Stack`, `Group`, `Text`, `Title`, `Card`. This is the DEFAULT. Every CSS property must be checked against style props FIRST.
2. **CSS modules** (`.module.css`) — ONLY for properties that Mantine style props genuinely cannot express: pseudo-selectors (`:hover`, `:focus`, `::before`), `box-shadow`, `border` shorthand, `animation`/`@keyframes`, complex selectors, `cursor`, `pointer-events`, `overflow`, `text-overflow`, `white-space`, `transition`.
3. **Inline styles ONLY for dynamic values** — `style={{ }}` is allowed only for truly dynamic runtime values (e.g., computed widths, positions, data-driven colors).
```

</details>
