---
name: indielayer__ui__skill
source: https://github.com/indielayer/ui/blob/7cf5b1d4a8ca99cd8e2de94f92c8a9e5123419da/.cursor/skills/add-component/SKILL.md
repo: indielayer/ui
kind: skill
stars: 223
last_pushed: 2026-05-26T10:04:58Z
license: mit
score: 8
domains: [web-frontend, ui-library]
tags: [vue, scaffolding, component-architecture, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# indielayer/ui — skill

**Why it's worth keeping:** It solves the 'ghost file' problem by explicitly listing all necessary registration steps and provides exact verification commands to ensure consistency.

**Summary:** Provides a strict blueprint for scaffolding, registering, and verifying new Vue components within a specific directory structure.

**Source credibility:** The source is an active, mid-sized open-source UI library with reasonable community traction.

**Recency:** Current; uses modern Vue 3 patterns (script setup) and contemporary tooling like pnpm.

**Source:** [indielayer/ui/.cursor/skills/add-component/SKILL.md](https://github.com/indielayer/ui/blob/7cf5b1d4a8ca99cd8e2de94f92c8a9e5123419da/.cursor/skills/add-component/SKILL.md) · 223★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: add-component
description: Add a new Vue component to @indielayer/ui with themes, tests, docs, and registry exports. Use when creating a new component, adding X-prefixed components, or scaffolding under packages/ui/src/components.
disable-model-invocation: true
---

# Add component

## Scaffold

Create `packages/ui/src/components/<name>/`:

- `<Name>.vue` — plain `<script lang="ts">` for props/types/`name: 'X<Name>'`, `<script setup>` for logic
- `index.ts` — `export { default as X<Name> }` and prop/theme types
- `theme/<Name>.base.theme.ts` and `theme/<Name>.carbon.theme.ts`
- `__tests__/<Name>.spec.ts`

## Register

1. `packages/ui/src/components/index.ts`
2. `packages/ui/src/themes/base/components.ts`
3. `packages/ui/src/themes/carbon/components.ts`

## Docs (if user-facing)

Follow the `docs-page` skill: `docs/pages/component/<name>/`.

## Verify

From repo root:

```bash
pnpm lint:ui
pnpm test:ci
```

Reference: `packages/ui/src/components/button/`
```

</details>
