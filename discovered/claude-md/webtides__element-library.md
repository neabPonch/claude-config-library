---
name: webtides__element-library
source: https://github.com/webtides/element-library/blob/2bfd126947194cfbb30ab112005f5982c5b7bd58/CLAUDE.MD
repo: webtides/element-library
kind: claude-md
stars: 5
last_pushed: 2026-06-15T09:40:46Z
license: mit
score: 9
domains: [web-frontend, ui-library]
tags: [web-components, architecture, ssr, tree-shaking]
curated: 2026-06-15
curated_by: config-scout
---

# webtides/element-library — claude-md

**Why it's worth keeping:** The 'Consumption Patterns' section provides critical intelligence on how to use the library without breaking tree-shaking or SSR; its structured 'Component Structure' creates a perfect blueprint for an AI to scaffold new components.

**Summary:** Provides deep architectural context for component imports, side-effect management, and SSR/client hydration strategies.

**Source credibility:** High technical depth despite low star count, suggesting professional-grade architecture expertise.

**Recency:** 

**Source:** [webtides/element-library/CLAUDE.MD](https://github.com/webtides/element-library/blob/2bfd126947194cfbb30ab112005f5982c5b7bd58/CLAUDE.MD) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.MD

This document provides context for AI assistants working with the `@webtides/element-library` codebase.

## Project Overview

`@webtides/element-library` is a collection of web components built with `@webtides/element-js`. The library provides pre-built custom elements with a focus on performance and accessibility.

- **Repository**: https://github.com/webtides/element-library
- **License**: MIT
- **Version**: 0.1.0
- **Status**: Work in progress - subject to breaking changes until 1.0 release

## Technology Stack

- **Framework**: `@webtides/element-js` (^1.2.11)
- **Build Tool**: Vite 8 (via Storybook; uses Rolldown bundler)
- **Testing**: Vitest 4 (with browser mode and custom test helpers)
- **Documentation**: Storybook 10.x
- **Linting**: ESLint (flat config) + Prettier
- **Node**: 20.19+ required (see `.nvmrc` and `engines.node`)
- **External Dependencies**:
    - `@glidejs/glide` for carousel functionality (pinned at `~3.6.2`; patched via `patch-package`)
    - `lozad` for lazy loading

## Project Structure

```
element-library/
├── src/
│   └── components/        # All web components
│       └── [component-name]/
│           ├── [component-name].js
```

</details>
