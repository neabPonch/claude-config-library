---
name: JetBrains__skills__skill
source: https://github.com/JetBrains/skills/blob/966a14a11f1d943411e4993a5a7567f9c1d045b7/vite/SKILL.md
repo: JetBrains/skills
kind: skill
stars: 234
last_pushed: 2026-05-20T14:04:13Z
license: unknown
score: 9
domains: [web-frontend, build-tools, javascript-ecosystem]
tags: [vite, bundler, frontend-dev, rolldown]
curated: 2026-06-16
curated_by: config-scout
---

# JetBrains/skills — skill

**Why it's worth keeping:** The use of a 'Preferences' section enforces architectural standards (ESM, TypeScript), while the hierarchical table structure allows an agent to quickly navigate from general config to advanced plugin API details.

**Summary:** A high-density configuration guide for Vite that includes specific focus on the upcoming Vite 8 and Rolldown migration. It provides structured lookup tables for core features, build/SSR modes, and environment APIs.

**Source credibility:** Extremely high; authored by Anthony Fu, a leading figure in the Vite/Vue ecosystem.

**Recency:** 

**Source:** [JetBrains/skills/vite/SKILL.md](https://github.com/JetBrains/skills/blob/966a14a11f1d943411e4993a5a7567f9c1d045b7/vite/SKILL.md) · 234★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: vite
description: Vite build tool configuration, plugin API, SSR, and Vite 8 Rolldown migration. Use when working with Vite projects, vite.config.ts, Vite plugins, or building libraries/SSR apps with Vite.
metadata:
  short-description: "Build and configure apps with Vite"
  author: Anthony Fu
  version: "2026.1.31"
  source: https://github.com/antfu/skills/tree/main/skills/vite
---

# Vite

> Based on Vite 8 beta (Rolldown-powered). Vite 8 uses Rolldown bundler and Oxc transformer.

Vite is a next-generation frontend build tool with fast dev server (native ESM + HMR) and optimized production builds.

## Preferences

- Use TypeScript: prefer `vite.config.ts`
- Always use ESM, avoid CommonJS

## Core

| Topic | Description | Reference |
|-------|-------------|-----------|
| Configuration | `vite.config.ts`, `defineConfig`, conditional configs, `loadEnv` | [core-config](references/core-config.md) |
| Features | `import.meta.glob`, asset queries (`?raw`, `?url`), `import.meta.env`, HMR API | [core-features](references/core-features.md) |
| Plugin API | Vite-specific hooks, virtual modules, plugin ordering | [core-plugin-api](references/core-plugin-api.md) |

## Build & SSR
```

</details>
