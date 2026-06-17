---
name: azerothcore__Keira3
source: https://github.com/azerothcore/Keira3/blob/4c11981c5ae1ec74302a643470dbaddcb0a5fa69/CLAUDE.md
repo: azerothcore/Keira3
kind: claude-md
stars: 422
last_pushed: 2026-06-09T17:35:37Z
license: agpl-3.0
score: 9
domains: [web-frontend, desktop-app]
tags: [angular, nx, architecture, testing]
curated: 2026-06-15
curated_by: config-scout
---

# azerothcore/Keira3 — claude-md

**Why it's worth keeping:** It excels at documenting abstract class hierarchies (the 'Editor pattern') and provides highly actionable, step-by-step checklists for adding new features. The inclusion of strict testing requirements and module boundary rules ensures AI-generated code adheres to project architecture.

**Summary:** This file provides exhaustive architectural context for an Angular/Nx monorepo, detailing complex inheritance patterns and strict module boundaries. It serves as a high-context technical manual that explains not just what the code does, but how to extend it following specific design patterns.

**Source credibility:** High; it is the official documentation for a well-maintained, starred open-source project (AzerothCore).

**Recency:** 

**Source:** [azerothcore/Keira3/CLAUDE.md](https://github.com/azerothcore/Keira3/blob/4c11981c5ae1ec74302a643470dbaddcb0a5fa69/CLAUDE.md) · 422★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Electron + Angular desktop DB editor for AzerothCore.

Scripts in `package.json`. `nx test <project>` / `nx lint <project>` scope to one lib (e.g. `keira-features-creature`).

## Repo layout

Nx monorepo. Apps in `apps/`, libs in `libs/`. Library names: `keira-<scope>-<name>`. Path aliases `@keira/<scope>/<name>` in `tsconfig.base.json` — always use these between libs, never relative paths.

Angular app is `apps/keira`. Routes table: `apps/keira/src/app/routes.ts`. Hash routing (`withHashLocation()`) — internal links must use `routerLink`. Routed components must be re-exported from the feature lib's `src/index.ts`.

Module boundaries enforced by `@nx/enforce-module-boundaries`:

```
app-keira → main-window → features → shared
```

A feature MUST NOT import another feature; move shared code to `libs/shared/`.

`libs/features/<name>/` — one lib per editor domain: `creature`, `quest`, `item`, `gameobject`, `spell`, `smart-scripts`, `conditions`, `gossip`, `trainer`, `texts`, `other-loots`, `dashboard`, `sql-editor`, `game-tele`, `unused-guid-search`.

`libs/main/{connection-window,main-window}/` — shell. Sidebar entries: `libs/main/main-window/src/sidebar/`.

`libs/shared
```

</details>
