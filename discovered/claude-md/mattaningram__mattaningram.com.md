---
name: mattaningram__mattaningram.com
source: https://github.com/mattaningram/mattaningram.com/blob/9babdb60b8ff2e1a4eaee17480abf3bdb2733731/CLAUDE.md
repo: mattaningram/mattaningram.com
kind: claude-md
stars: 2
last_pushed: 2026-05-17T15:17:53Z
license: unknown
score: 9
domains: [web-frontend, astro, css]
tags: [astro, component-architecture, animations, css]
curated: 2026-06-16
curated_by: config-scout
---

# mattaningram/mattaningram.com — claude-md

**Why it's worth keeping:** Includes high-density technical rules like specific `animation-fill-mode` usage to prevent visual bugs and a strict pattern for handling component props and positioning. The separation of motion from base components is a professional-grade design rule that prevents 'magic' side effects.

**Summary:** Highly opinionated architectural guidelines for an Astro-based frontend, focusing on component structure and CSS animation mechanics.

**Source credibility:** Personal site project; quality reflects high-level frontend engineering standards.

**Recency:** Current, with updates as recent as one month ago.

**Source:** [mattaningram/mattaningram.com/CLAUDE.md](https://github.com/mattaningram/mattaningram.com/blob/9babdb60b8ff2e1a4eaee17480abf3bdb2733731/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Rules

- Do not add unnecessary text or styling unless it is explicitly requested.
- Default to on device features and libraries and packages that give access to on device features.
- Componentize anything used in more than 3 places, particular basic UI components like buttons and inputs, but not simple layouts.
- Do not switch to a different library or package unless it is explicitly requested.
- Do not add styles to existing elements or components unless explicity requested.
- Nest `@media` rules inside their parent selector instead of using separate top-level `@media` blocks.
- When refactoring or moving code between files, preserve the exact original behavior including animation values, timing, and spring configurations. Do not "improve" or change values.
- Keep reusable components simple and animation-free. Apply animations at the usage site, not inside the component itself. This allows the same component to be used with different animations in different contexts.
- Do not add positioning styles (margin, padding, absolute/relative positioning) to reusable components. These should always be set where the component is used, since positioning requirements vary by context.
- Whe
```

</details>
