---
name: massCodeIO__massCode__skill
source: https://github.com/massCodeIO/massCode/blob/1a8067342201fc5d5ac096db7b8d703603a7881d/.agents/skills/vue-renderer-standards/SKILL.md
repo: massCodeIO/massCode
kind: skill
stars: 6828
last_pushed: 2026-06-13T05:15:18Z
license: agpl-3.0
score: 8
domains: [web-frontend, electron-desktop-apps, architecture-standards]
tags: [vue3, electron, composition-api, architectural-constraints]
curated: 2026-06-15
curated_by: config-scout
---

# massCodeIO/massCode — skill

**Why it's worth keeping:** The explicit 'Manual Imports Only Where Required' list prevents AI hallucination of boilerplate imports; the strict boundary enforcement prevents unauthorized Node.js calls in the renderer.

**Summary:** Defines architectural boundaries and coding patterns for a Vue 3 renderer within an Electron application. It specifies auto-import rules, state management patterns, and security constraints between the UI and backend.

**Source credibility:** High-quality source with 6.8k stars and active maintenance.

**Recency:** 

**Source:** [massCodeIO/massCode/.agents/skills/vue-renderer-standards/SKILL.md](https://github.com/massCodeIO/massCode/blob/1a8067342201fc5d5ac096db7b8d703603a7881d/.agents/skills/vue-renderer-standards/SKILL.md) · 6828★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: vue-renderer-standards
description: Use when editing massCode renderer code in Vue 3, especially for script setup patterns, import rules, composables, shared state, and renderer-side conventions.
---

# Vue Renderer Standards

## Overview

Renderer в massCode строится на Vue 3 Composition API с `<script setup lang="ts">`. Здесь важны строгие import rules, composable-first state sharing и запрет на прямой доступ к backend-возможностям.

## Component Pattern

- Используй Vue 3 Composition API и `<script setup lang="ts">`.
- Vue core (`ref`, `computed`, `watch`, `onMounted` и подобные) не импортируй вручную: они auto-imported.
- Проектные компоненты из `src/renderer/components/` тоже не импортируй вручную: они auto-imported.
- Локальную логику компонента держи в script, а не в template.

## Manual Imports Only Where Required

Всегда импортируй вручную:

- composables из `@/composables`;
- utils из `@/utils`;
- `@vueuse/core`;
- Electron bridge из `@/electron`;
- Shadcn UI из `@/components/ui/shadcn/*`.

## Shared State

- Глобальное shared state реализуется composables без Pinia/Vuex.
- Reactive state, который должен шариться между компонентами, объявляй на module level, вне
```

</details>
