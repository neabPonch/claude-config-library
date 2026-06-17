---
name: kskwtnk__portfolio
source: https://github.com/kskwtnk/portfolio/blob/f701dd1db7548c393850460f0818926fa4147dae/CLAUDE.md
repo: kskwtnk/portfolio
kind: claude-md
stars: 15
last_pushed: 2026-05-14T23:25:57Z
license: unknown
score: 8
domains: [web-frontend, astro]
tags: [astro, tailwind-v4, biome, japanese]
curated: 2026-06-16
curated_by: config-scout
---

# kskwtnk/portfolio — claude-md

**Why it's worth keeping:** The 'Gotchas' section provides actionable workarounds for tool limitations (Biome/Astro), and it explicitly explains custom content loader logic to prevent the AI from misinterpreting data flow.

**Summary:** A highly specific guide for an Astro-based portfolio that covers language constraints, command workflows, and architectural nuances.

**Source credibility:** Personal portfolio project; high specificity indicates a highly tailored, practical config.

**Recency:** Very recent (1 month ago) and utilizes modern tool versions like Tailwind v4.

**Source:** [kskwtnk/portfolio/CLAUDE.md](https://github.com/kskwtnk/portfolio/blob/f701dd1db7548c393850460f0818926fa4147dae/CLAUDE.md) · 15★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Astro-based portfolio site for Keisuke Watanuki. All website content is in Japanese.

## Language

- Always respond to the user in Japanese
- Keep code comments and commit messages in English

## Commands

Package manager: `pnpm`

- `pnpm dev` - Start dev server (localhost:4321)
- `pnpm build` - Production build to `./dist/`
- `pnpm check` - Run all Biome checks (lint + format + assist)
- `pnpm check:fix` - Auto-fix all Biome issues

Always run `pnpm check` after making changes to verify code quality.

## Architecture

### Content Collections

Content schemas are defined in `src/content.config.ts`. The `qiita-articles` collection uses a custom loader that fetches from the Qiita API at build time — see `src/content.config.ts` for the loader implementation with timeout and error handling.

### 3D Background Effect

`src/effects/granyGradients.ts` renders animated gradient effects using Three.js with custom GLSL shaders (`src/effects/*.glsl`). These run on the homepage only.

### Styling

TailwindCSS v4 via Vite plugin. Typography uses Shippori Mincho font family for Japanese content.

## Gotchas

- Biome's VSCode extension does not reliably format `.astro` files on save
```

</details>
