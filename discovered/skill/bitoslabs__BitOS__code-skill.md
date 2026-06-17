---
name: bitoslabs__BitOS__code-skill
source: https://github.com/bitoslabs/BitOS/blob/9a6560b59f9571ab99c2633a94833eb4da9c02f4/.agent/code-SKILL.md
repo: bitoslabs/BitOS
kind: skill
stars: 2
last_pushed: 2026-03-05T04:18:40Z
license: unknown
score: 8
domains: [web-frontend, vue-nuxt]
tags: [nuxt, vue, typescript, ui-patterns, infinite-scroll]
curated: 2026-06-15
curated_by: config-scout
---

# bitoslabs/BitOS — skill

**Why it's worth keeping:** The 'Easy Scroll' Intersection Observer pattern is a high-quality, production-ready implementation that prevents common infinite scroll bugs. It also provides clear structural constraints for separating business logic into composables versus services.

**Summary:** A comprehensive coding standard for Nuxt 3 and Vue 3 projects covering architecture, naming, and UI patterns.

**Source credibility:** Low star count but recent activity and highly specific, professional-grade implementation patterns.

**Recency:** Very current; uses modern Nuxt 3 and Vue Composition API standards.

**Source:** [bitoslabs/BitOS/.agent/code-SKILL.md](https://github.com/bitoslabs/BitOS/blob/9a6560b59f9571ab99c2633a94833eb4da9c02f4/.agent/code-SKILL.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: BitOS Social Coding Style
description: Best practices, patterns, and conventions for the BitOS Social Nuxt project.
metadata:
  author: BitOS Team
  version: "2026.2.1"
  stack: Nuxt 3, Vue 3, Tailwind CSS
---

# BitOS Social Coding Standards

This skill defines the coding style and best practices for the BitOS Social project. Always refer to this when writing or refactoring code to ensure consistency and maintainability.

## Preferences

- **Framework**: Prefer **Nuxt 3** features over vanilla Vue where applicable.
- **Language**: Strictly **TypeScript**. Avoid `any`.
- **API Style**: Always use **Composition API** with `<script setup lang="ts">`.
- **Styling**: Use **Tailwind CSS** / **UnoCSS** utility classes. Avoid scoped CSS unless necessary for complex animations.
- **Icons**: Use `@nuxt/icon` module (e.g., `heroicons:`, `svg-spinners:`).

## Core Architecture

The project follows a standard Nuxt 3 directory structure within the `app/` directory:

- **`app/pages/`**: Route views. Should primarily coordinate data fetching and layout. Keep logic minimal.
- **`app/components/`**: Reusable UI elements.
  - Prefer generic components (e.g., `CommonLineChart`, `UButton`) f
```

</details>
