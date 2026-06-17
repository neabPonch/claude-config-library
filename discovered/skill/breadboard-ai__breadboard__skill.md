---
name: breadboard-ai__breadboard__skill
source: https://github.com/breadboard-ai/breadboard/blob/2aa335975f8c43a1f564193812a687d0f476819c/spikes/ea-magazine/skill.md
repo: breadboard-ai/breadboard
kind: skill
stars: 405
last_pushed: 2026-06-11T14:26:27Z
license: apache-2.0
score: 9
domains: [web-frontend, ui-ux, generative-ai]
tags: [editorial-design, layout-rules, art-direction]
curated: 2026-06-15
curated_by: config-scout
---

# breadboard-ai/breadboard — skill

**Why it's worth keeping:** Uses 'Critical Anti-Patterns' to define what NOT to do, alongside specific CSS/layout techniques like asymmetric columns and text layering. This is a masterclass in using negative constraints to steer creative output.

**Summary:** Provides highly opinionated art direction rules to transform raw data into sophisticated, magazine-style editorial layouts. It explicitly prevents common AI UI failures like the 'generic card grid' pattern.

**Source credibility:** High; breadboard-ai is an active, specialized library for generative prototyping.

**Recency:** Extremely current, utilizing modern design tokens and layout logic.

**Source:** [breadboard-ai/breadboard/spikes/ea-magazine/skill.md](https://github.com/breadboard-ai/breadboard/blob/2aa335975f8c43a1f564193812a687d0f476819c/spikes/ea-magazine/skill.md) · 405★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: Editorial Briefing
description:
  Art direction for presenting user data as a personal morning briefing.
  Defines editorial techniques, layout sections, anti-patterns, and tone.
  Technical infrastructure comes from the UI Skill, not this file.
---

# Editorial Briefing Skill

Present the user's active playbooks as a personal morning briefing — an
**editorial layout** with high-end magazine art direction — warm, confident,
unhurried.

## CRITICAL Anti-Patterns — NEVER DO THESE

These are the patterns that make outputs look generic and boring.
**Violating any of these is a failure.**

1. **NO GRID OF CARDS.** Never render all playbooks as same-sized cards in a
   CSS grid or flexbox wrap. This is a dashboard, not a briefing. Each item
   must receive treatment proportional to its urgency and narrative weight.

2. **NO UNIFORM COMPONENTS.** You must NOT render all playbooks using the
   same component at different sizes. Urgent items, feature items, progress
   items, and quiet items MUST use fundamentally different visual treatments.

3. **NO CARD BORDERS OR SHADOWS.** Do not put cards in rounded-rectangle
   containers with shadows. Content should float on the page, sepa
```

</details>
