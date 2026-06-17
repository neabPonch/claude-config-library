---
name: Tresjs__tres
source: https://github.com/Tresjs/tres/blob/01c12e85bcc051f55b01d938c22fb8b7afe36ffe/CLAUDE.md
repo: Tresjs/tres
kind: claude-md
stars: 3592
last_pushed: 2026-06-16T13:42:20Z
license: mit
score: 8
domains: [web-frontend, 3d-graphics]
tags: [monorepo, documentation-protocol, threejs]
curated: 2026-06-16
curated_by: config-scout
---

# Tresjs/tres — claude-md

**Why it's worth keeping:** The instruction to proactively search for `llms.txt` or `llms-full.txt` is an elite pattern that significantly reduces hallucinations in modern web development.

**Summary:** Provides essential monorepo mapping and a sophisticated documentation retrieval protocol.

**Source credibility:** High; TresJS is a highly starred, actively maintained library within the Vue ecosystem.

**Recency:** Very current, leveraging emerging documentation standards like llms.txt.

**Source:** [Tresjs/tres/CLAUDE.md](https://github.com/Tresjs/tres/blob/01c12e85bcc051f55b01d938c22fb8b7afe36ffe/CLAUDE.md) · 3592★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

TresJS is a Vue-based declarative 3D custom renderer for Three.js

## Key Packages

- **@tresjs/core** (`packages/core`): The core library implementing the Vue custom renderer for Three.js
- **@tresjs/cientos** (`packages/cientos`): Collection of helpers and abstractions (controls, loaders, staging, materials, shapes)
- **@tresjs/post-processing** (`packages/postprocessing`): Post-processing effects library built on pmndrs/postprocessing
- **@tresjs/leches** (`packages/leches`): Tasty GUI for Vue controls 🍰
- **@tresjs/eslint-config** (`packages/eslint-config`): Shared ESLint configuration for the ecosystem
- **@tresjs/nuxt** (`packages/nuxt`): Nuxt module integration


## Versioning

Version increments follow conventional commits:
- `feat:` → minor bump
- `fix:` → patch bump
- `BREAKING CHANGE:` or `feat!:` → major bump


### Workspace Dependencies
Packages use pnpm's `workspace:*` protocol for internal dependencies. The catalog in `pnpm-workspace.yaml` manages shared dependency versions (Three.js, Vue, Vite, etc.).

## Research & Documentation

- **NEVER hallucinate or guess URLs**
- ALWAYS try accessing the `llms.txt` or `llms-full.txt` file first to find relevant d
```

</details>
