---
name: redis__RedisInsight__skill
source: https://github.com/redis/RedisInsight/blob/f3b84c627cf7e84048494482b98d59fa071d22d8/.ai/skills/tsconfigs/SKILL.md
repo: redis/RedisInsight
kind: skill
stars: 8536
last_pushed: 2026-06-16T06:31:53Z
license: other
score: 9
domains: [monorepo, typescript, build-systems]
tags: [tsconfig, webpack, eslint, path-aliases, node-js]
curated: 2026-06-16
curated_by: config-scout
---

# redis/RedisInsight — skill

**Why it's worth keeping:** It details critical cross-referencing requirements for path aliases (TS vs. Webpack) and specific constraints regarding Node 22 ESM/CommonJS compatibility.

**Summary:** Provides a detailed map of a distributed TypeScript configuration architecture across UI, API, and Desktop layers.

**Source credibility:** High; based on a major, highly-starred open source project (RedisInsight).

**Recency:** Current; specifically addresses modern Node 22 module resolution behavior.

**Source:** [redis/RedisInsight/.ai/skills/tsconfigs/SKILL.md](https://github.com/redis/RedisInsight/blob/f3b84c627cf7e84048494482b98d59fa071d22d8/.ai/skills/tsconfigs/SKILL.md) · 8536★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: tsconfigs
description: >-
  Locate and modify TypeScript configuration in RedisInsight. Use when adding
  path aliases, introducing a new TS area, debugging webpack/ts-node/ESLint
  path resolution, or the user asks about tsconfig, path mappings, or where
  TypeScript is configured.
---

# TypeScript Configuration

RedisInsight has no root `tsconfig.json`. Config is split per area, each owning its own paths, includes, and consumers. ESLint uses `parserOptions.project: true` to auto-discover the nearest tsconfig for each linted file.

## Layout

| File | Owns | Consumers |
| - | - | - |
| `redisinsight/ui/tsconfig.json` | UI source, `uiSrc/*`, `apiClient` paths | Vite (UI build), ESLint UI override, `yarn type-check:ui` |
| `redisinsight/api/tsconfig.json` | API source, `src/*`, `tests/*` paths | NestJS build, ESLint API override |
| `redisinsight/api/tsconfig.check.json` | Same as base + `strict: true` (with `strictPropertyInitialization` and `useUnknownInCatchVariables` off) and `noEmit: true` | `yarn type-check:api` only — kept separate so strict mode doesn't break `nest build`. See the `type-check-baselines` skill. |
| `redisinsight/desktop/tsconfig.json` | Desktop sou
```

</details>
