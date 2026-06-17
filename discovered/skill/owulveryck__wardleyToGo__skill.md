---
name: owulveryck__wardleyToGo__skill
source: https://github.com/owulveryck/wardleyToGo/blob/a31d299ed0100ace9c7ab9513a6b87b10bfc4ea3/wtg2/skill.md
repo: owulveryck/wardleyToGo
kind: skill
stars: 57
last_pushed: 2026-06-10T18:50:41Z
license: mit
score: 9
domains: [strategy, business-analysis, systems-thinking]
tags: [wardley-maps, strategic-planning, dsl]
curated: 2026-06-14
curated_by: config-scout
---

# owulveryck/wardleyToGo — skill

**Why it's worth keeping:** It embeds high-level strategic frameworks (Manoeuvre vs Tactique) and diagnostic patterns (Flow Anomalies) rather than just syntax, allowing the agent to perform actual analysis instead of just rendering shapes.

**Summary:** Turns Claude into a strategic consultant capable of generating complex Wardley Maps using the WTG2 DSL. It provides high-level semantic meaning to diagrams through specialized annotations.

**Source credibility:** High quality; active repository with specific domain expertise in strategic mapping.

**Recency:** Very current, updated within the last month.

**Source:** [owulveryck/wardleyToGo/wtg2/skill.md](https://github.com/owulveryck/wardleyToGo/blob/a31d299ed0100ace9c7ab9513a6b87b10bfc4ea3/wtg2/skill.md) · 57★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: wtg2
description: Generate Wardley Maps in the WTG2 domain-specific language. Use when the user asks to create, design, or describe a Wardley Map, or asks about strategic mapping.
argument-hint: [description of the map to generate]
---

# WTG2 — Wardley Map Language

You are generating Wardley Maps in the **WTG2** domain-specific language. Your output must be a valid `.wtg2` file that can be parsed and rendered to SVG.

---

## What is a Wardley Map?

A Wardley Map is a strategic tool that visualizes a **value chain** (vertical axis) against the **evolution** of each component (horizontal axis).

- **Value chain (Y axis):** Components at the top are directly visible to the user/customer. Components lower down are dependencies — infrastructure, platforms, data sources.
- **Evolution (X axis):** Components move left-to-right through four phases as they mature:
  1. **Genesis** (I) — Novel, poorly understood, high uncertainty
  2. **Custom-built** (II) — Understood but bespoke, requires expertise
  3. **Product/Rental** (III) — Increasingly standardized, available as products
  4. **Commodity/Utility** (IV) — Highly standardized, pay-per-use, invisible

Key principles:
- **A
```

</details>
