---
name: jayanthmb14__forthepeople__district-expansion-skill
source: https://github.com/jayanthmb14/forthepeople/blob/38df95893a3752585d4d8ae00e3d88474287e0f9/docs/DISTRICT-EXPANSION-SKILL.md
repo: jayanthmb14/forthepeople
kind: skill
stars: 263
last_pushed: 2026-06-11T17:59:30Z
license: other
score: 9
domains: [data-seeding, domain-specific-knowledge, scaling-automation]
tags: [india, civic-tech, database-seeding]
curated: 2026-06-15
curated_by: config-scout
---

# jayanthmb14/forthepeople — skill

**Why it's worth keeping:** Demonstrates how to use domain-specific hierarchies and 'local adaptation' logic to automate complex database seeding and scraper configurations.

**Summary:** Provides highly dense, structured ground truth for scaling a civic transparency platform across new geographical districts.

**Source credibility:** High; 263 stars indicate established utility in the Indian civic-tech space.

**Recency:** Current; contains up-to-date infrastructure estimates for 2025-26.

**Source:** [jayanthmb14/forthepeople/docs/DISTRICT-EXPANSION-SKILL.md](https://github.com/jayanthmb14/forthepeople/blob/38df95893a3752585d4d8ae00e3d88474287e0f9/docs/DISTRICT-EXPANSION-SKILL.md) · 263★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: forthepeople-district-expansion
description: "Skill for expanding ForThePeople.in to new districts. Use when adding Bengaluru Urban, Mysuru, or any new Indian district to the platform. Triggers: 'add district', 'expand to Bangalore', 'expand to Mysore', 'unlock district', 'new city', 'seed data for district', 'add Bengaluru', 'add Mysuru', 'district-specific modules', 'local industry module'. Covers: district hierarchy seeding, taluk data, unique local modules (IT parks for Bangalore, tourism/heritage for Mysore, sugar for Mandya), infrastructure projects seeding, famous personalities, leadership data, GeoJSON maps, scraper configuration, and AI news intelligence expansion."
---

# ForThePeople.in — District Expansion Skill

## Expansion Philosophy

The codebase is GENERIC. Every district uses the same 29 dashboard modules, same API routes, same UI components. Expanding to a new district requires:

1. **Database seeding** — Add State/District/Taluk/Village rows with `active: true`
2. **Data population** — Seed ALL 45+ Prisma models with real data for the new district
3. **Local industry adaptation** — The "Local Industries" module adapts per district (Sugar→Mandya, IT Par
```

</details>
