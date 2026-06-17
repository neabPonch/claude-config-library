---
name: tagspaces__tagspaces
source: https://github.com/tagspaces/tagspaces/blob/100e78e1a85a74649a246ee1e01cadb6ddcd6e2b/CLAUDE.md
repo: tagspaces/tagspaces
kind: claude-md
stars: 5167
last_pushed: 2026-06-14T12:06:33Z
license: agpl-3.0
score: 9
domains: [desktop-app, file-management, monorepo]
tags: [electron, typescript, indexing, architecture-guide]
curated: 2026-06-15
curated_by: config-scout
---

# tagspaces/tagspaces — claude-md

**Why it's worth keeping:** It uses 'gotchas' to prevent subtle bugs like cache invalidation issues and explicitly lists key utility functions so the agent doesn't reinvent existing path or tag-parsing logic.

**Summary:** This file provides an exhaustive map of a complex monorepo, covering architectural splits (Main vs. Renderer), detailed filesystem metadata structures, and intricate indexing logic.

**Source credibility:** High; a well-maintained repository with significant community adoption (5k+ stars).

**Recency:** Very recent/current, showing high relevance to modern development workflows.

**Source:** [tagspaces/tagspaces/CLAUDE.md](https://github.com/tagspaces/tagspaces/blob/100e78e1a85a74649a246ee1e01cadb6ddcd6e2b/CLAUDE.md) · 5167★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build & Development

- **Install dependencies**: `npm install`
- **Run development (Electron)**: `npm run dev`
- **Build production**: `npm run build`
- **Lint**: `npm run lint`
- **Run all tests**: `npm run test`
- **Run a single test**: `npx jest path/to/test.ts`

## Architecture

- **Electron app** with renderer (React/TypeScript) and main process
- **Renderer source**: `src/renderer/` — React components, hooks, services
- **Main process**: `src/main/` — Electron main process, IPC handlers
- **Locales**: `src/renderer/locales/{lang}/core.json` — i18n translations (i18next with `core` namespace)
- **Extensions**: loaded from `release/app/node_modules/@tagspaces/extensions/`
- **Perspectives**: different views for folder content (Grid, List, Kanban, Gallery, Mapique, FolderViz, Calendar)
- **State management**: Redux with slices in `src/renderer/reducers/`

## tagspaces-common Monorepo (`../tagspaces-common`)

Lerna-managed monorepo (`packages/*`) providing shared libraries. Version 4.6.1. Key packages:

### @tagspaces/tagspaces-common (`packages/common`)

Core u
```

</details>
