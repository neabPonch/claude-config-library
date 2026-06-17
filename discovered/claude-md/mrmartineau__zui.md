---
name: mrmartineau__zui
source: https://github.com/mrmartineau/zui/blob/d0c284c18c92c80af7cc20ad4a84181601b9f038/claude.md
repo: mrmartineau/zui
kind: claude-md
stars: 1
last_pushed: 2026-06-15T22:11:52Z
license: isc
score: 9
domains: [web-frontend, css-architecture, ui-library]
tags: [design-tokens, monorepo, component-architecture]
curated: 2026-06-16
curated_by: config-scout
---

# mrmartineau/zui — claude-md

**Why it's worth keeping:** Provides exact file paths for design tokens to prevent duplication and defines a clear recipe for creating consistent components across multiple framework wrappers (React, Astro, Vue, etc.).

**Summary:** Establishes strict architectural protocols for a multi-framework CSS UI library, including documentation and component creation workflows.

**Source credibility:** Well-structured single-author project with very recent activity.

**Recency:** Highly current; uses modern CSS standards like oklch and light-dark().

**Source:** [mrmartineau/zui/claude.md](https://github.com/mrmartineau/zui/blob/d0c284c18c92c80af7cc20ad4a84181601b9f038/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ZUI — Claude Guidelines

## Project Overview

ZUI is a CSS-first UI library (`@mrmartineau/zui`) with optional React, Astro, Solid, Svelte, and Vue component wrappers. See `AGENTS.md` for full architecture and conventions — everything there applies here too.

## Critical Rules

1. **Update the docs site.** Any new component, token, utility, or API change must be reflected in the Astro docs site at `docs/`. Create or update the relevant `.mdx` page and add sidebar entries in `docs/src/components/Sidebar.astro`.

2. **Reuse existing styles, tokens, and components.** Before writing new CSS or creating new helpers, check:
   - `packages/zui/src/css/tokens/` for design tokens (`--space-*`, `--color-*`, `--radius-*`, `--shadow-*`, `--step-*`, `--ease-*`, `--z-*`, etc.)
   - `packages/zui/src/css/theme.css` for semantic tokens (`--color-text`, `--color-background`, `--color-surface`, `--color-border`, `--color-theme`, `--color-accent`)
   - `packages/zui/src/css/utilities/` for utility classes
   - `packages/zui/src/css/components/` for existing component styles
   - `docs/src/components/` for existing demo helpers (`Demo`, `CodeTabs`, `ButtonRow`, `TokenGrid`, etc.)

3. **Use Phosphor
```

</details>
