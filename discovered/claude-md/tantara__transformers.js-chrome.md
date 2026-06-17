---
name: tantara__transformers.js-chrome
source: https://github.com/tantara/transformers.js-chrome/blob/fa7b7b97d4d0e0a999bf6429cde57811b2ad306d/CLAUDE.md
repo: tantara/transformers.js-chrome
kind: claude-md
stars: 103
last_pushed: 2026-03-22T22:30:01Z
license: apache-2.0
score: 9
domains: [web-extensions, monorepo, ai-inference, frontend]
tags: [monorepo, browser-extension, webgpu, build-hacks]
curated: 2026-06-15
curated_by: config-scout
---

# tantara/transformers.js-chrome — claude-md

**Why it's worth keeping:** It documents critical 'hidden' knowledge, such as mandatory module stubs and post-build scripts required to make Node-centric code run in a browser. This prevents the AI from introducing breaking changes to the delicate build process.

**Summary:** A comprehensive technical guide for a complex monorepo involving local AI inference and browser extensions. It bridges the gap between high-level command usage and low-level build-time environment requirements.

**Source credibility:** High; specialized repository with recent updates and clear technical depth in WebGPU/on-device AI.

**Recency:** Highly current, referencing Next.js 15 and Expo SDK 54.

**Source:** [tantara/transformers.js-chrome/CLAUDE.md](https://github.com/tantara/transformers.js-chrome/blob/fa7b7b97d4d0e0a999bf6429cde57811b2ad306d/CLAUDE.md) · 103★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Monorepo for on-device AI inference apps. Uses [Turborepo](https://turborepo.com) with pnpm workspaces.

### Apps

- `apps/plasmo` — Browser extension (Chrome MV3, Firefox MV2, Safari) running LLM inference locally via Transformers.js and WebGPU
- `apps/nextjs` — Next.js 15 web app
- `apps/expo` — Expo SDK 54 / React Native mobile app
- `apps/tanstack-start` — Tanstack Start web app

### Shared Packages

- `packages/api` — tRPC v11 router
- `packages/auth` — Authentication (better-auth)
- `packages/db` — Database (Drizzle + Supabase)
- `packages/ui` — Shared UI components (shadcn-ui)
- `tooling/` — Shared eslint, prettier, tailwind, typescript configs

## Commands

```bash
# Monorepo root
pnpm dev              # Run all apps
pnpm dev:chrome       # Run plasmo Chrome extension only
pnpm dev:firefox      # Run plasmo Firefox extension only
pnpm dev:plasmo       # Run both Chrome + Firefox via Turbo TUI
pnpm dev:next         # Run Next.js app only

# Inside apps/plasmo
pnpm dev              # Start dev server → build/chrome-mv3-dev/
pnpm dev:chrome
```

</details>
