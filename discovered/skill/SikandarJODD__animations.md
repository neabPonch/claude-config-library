---
name: SikandarJODD__animations
source: https://github.com/SikandarJODD/animations/blob/5dc6e9bb20ac938e74b558141e905c2d12eff99d/SKILL.md
repo: SikandarJODD/animations
kind: skill
stars: 243
last_pushed: 2026-06-13T06:22:51Z
license: mit
score: 9
domains: [web-frontend, ui-development]
tags: [svelte, animations, motion-sv, layout-engine]
curated: 2026-06-15
curated_by: config-scout
---

# SikandarJODD/animations — skill

**Why it's worth keeping:** It highlights non-obvious requirements like mandatory object-syntax for styles and the specific createLayoutMotion pattern required to avoid layout bugs in Svelte.

**Summary:** Provides specialized patterns and critical technical gotchas for using the motion-sv library within Svelte 5 environments.

**Source credibility:** High; the source is a specialized animation repository with significant stars and very recent updates.

**Recency:** 

**Source:** [SikandarJODD/animations/SKILL.md](https://github.com/SikandarJODD/animations/blob/5dc6e9bb20ac938e74b558141e905c2d12eff99d/SKILL.md) · 243★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: motion-sv
description: Documentation and patterns for using motion-sv, a Svelte 5 port of Motion (Framer Motion). Use this when the user wants animations, gestures, or transitions in Svelte.
---

# Motion for Svelte (motion-sv)

A port of the Motion library (formerly Framer Motion) specifically for Svelte 5. It aligns closely with the **motion-v** API structure rather than the React version.

## Stack Requirements

- MUST be used with Svelte 5 (Runes).
- Package name: `motion-sv`.

## Core Components

### `motion`

The primary component factory. Use dot notation to render **any** HTML element.

```svelte
<script>
  import { motion } from "motion-sv";
</script>

<!-- Sections & Headings -->
<motion.section initial={{ opacity: 0 }} animate={{ opacity: 1 }}>
  <motion.h1 animate={{ y: 0 }}>Headline</motion.h1>
</motion.section>

<!-- Links & Buttons -->
<motion.a
  href="/about"
  whileHover={{ scale: 1.05 }}
  whilePress={{ scale: 0.95 }}
>
  Go to About
</motion.a>
```

### Styling Pattern (Important)

ALWAYS pass styles as an object via `style={{ key: value }}`, never as a string. This is required to bind `MotionValue`s correctly without triggering re-renders.

```svelte
```

</details>
