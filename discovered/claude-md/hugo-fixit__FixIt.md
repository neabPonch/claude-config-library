---
name: hugo-fixit__FixIt
source: https://github.com/hugo-fixit/FixIt/blob/6070061b6b9d63a1cb5973abd1dc56a747a64ddc/CLAUDE.md
repo: hugo-fixit/FixIt
kind: claude-md
stars: 1109
last_pushed: 2026-06-15T08:30:08Z
license: mit
score: 9
domains: [web-frontend, static-site-generator]
tags: [monorepo, architecture-heavy, typescript, hugo]
curated: 2026-06-15
curated_by: config-scout
---

# hugo-fixit/FixIt — claude-md

**Why it's worth keeping:** The documentation of the module-to-module communication via an event bus and strict dependency injection rules prevents AI from introducing side effects or breaking architecture.

**Summary:** Provides an exhaustive architectural blueprint and specific implementation standards for a complex Hugo/TypeScript monorepo.

**Source credibility:** High; part of a popular, actively maintained (last pushed 0 months ago) Hugo theme with over 1k stars.

**Recency:** Highly current, utilizing modern tooling like pnpm, TypeScript, and latest ES6 private fields.

**Source:** [hugo-fixit/FixIt/CLAUDE.md](https://github.com/hugo-fixit/FixIt/blob/6070061b6b9d63a1cb5973abd1dc56a747a64ddc/CLAUDE.md) · 1109★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

FixIt is a modern, responsive theme for the Hugo static site generator. Built with Hugo templates, SCSS, and TypeScript.

## Development Commands

### Prerequisites

- Node.js >= 20
- Hugo Extended >= 0.158.0 (Dart Sass required)
- pnpm

### Development

```bash
pnpm install           # Install dependencies
pnpm dev:demo          # Start demo site dev server
pnpm dev:test          # Start test site dev server
pnpm dev:docs          # Start docs dev server (requires fixit-docs as sibling directory)
```

### Build

```bash
pnpm build:demo        # Build demo site
pnpm build:test        # Build test site
pnpm build             # Build all sites (demo + test, merged into public/)
pnpm preview           # Preview built site (requires build first)
```

### Code Generation

```bash
pnpm gen:lexers        # Regenerate assets/scss/core/maps/_chroma-lexers.scss from Chroma source
```

### Code Quality

```bash
pnpm lint              # Run ESLint
pnpm typecheck         # Run TypeScript type checking
```

There are no unit tests. Verify changes by building `
```

</details>
