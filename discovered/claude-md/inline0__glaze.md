---
name: inline0__glaze
source: https://github.com/inline0/glaze/blob/23a1526349ecec93602f8e8b7b643717d8854363/CLAUDE.md
repo: inline0/glaze
kind: claude-md
stars: 693
last_pushed: 2026-03-26T13:57:07Z
license: other
score: 9
domains: [web-frontend, animation-framework]
tags: [monorepo, typescript, gsap, bun]
curated: 2026-06-15
curated_by: config-scout
---

# inline0/glaze — claude-md

**Why it's worth keeping:** It provides explicit mappings between utility files and their specific purposes, alongside a detailed 'Animation Flow' which is critical for AI understanding of complex logic pipelines.

**Summary:** A high-density technical specification that maps monorepo structure, command patterns, and internal logic flows.

**Source credibility:** Strong; established open-source project with significant stars and recent activity.

**Recency:** 

**Source:** [inline0/glaze/CLAUDE.md](https://github.com/inline0/glaze/blob/23a1526349ecec93602f8e8b7b643717d8854363/CLAUDE.md) · 693★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Glaze

Utility-based animations for the web. A declarative animation syntax that converts data attributes into GSAP timeline operations.

## Project Overview

Glaze parses animation strings from `data-animate` attributes and converts them into GSAP animations. It provides a utility-class-like syntax for animations, similar to how Tailwind CSS works for styling.

**Package name:** `glazejs`
**Version:** 2.0.1
**License:** MIT
**Homepage:** https://glaze.dev

---

## Monorepo Structure

```
glaze/
├── packages/core/           # Main library (published as glazejs)
│   ├── src/
│   │   ├── index.ts        # Main entry (~528 lines)
│   │   ├── types.ts        # Type definitions
│   │   └── utils/          # 11 utility files
│   ├── tests/
│   │   ├── unit/           # Vitest unit tests
│   │   └── e2e/            # Playwright E2E tests
│   ├── dist/               # Build output (ES module)
│   ├── scripts/
│   │   └── postbuild.js    # Minification + file copying
│   ├── vite.config.ts
│   └── vitest.config.unit.ts
├── apps/docs/              # Documentation site (Next.js + OneDocs)
│   ├── src/app/            # Next.js App Router
│   ├── content/docs/       # MDX documentation (11 fi
```

</details>
