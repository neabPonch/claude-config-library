---
name: ever-co__ever-teams
source: https://github.com/ever-co/ever-teams/blob/335bfe2fd5680fbaf303df111bbd50b729a670ae/CLAUDE.md
repo: ever-co/ever-teams
kind: claude-md
stars: 509
last_pushed: 2026-06-16T11:10:30Z
license: agpl-3.0
score: 9
domains: [web-frontend, monorepo, fullstack]
tags: [nextjs, monorepo, yarn-workspaces, typescript]
curated: 2026-06-17
curated_by: config-scout
---

# ever-co/ever-teams — claude-md

**Why it's worth keeping:** The granular directory mappings and specific authentication service/endpoint details prevent AI guesswork in large-scale codebases. It also includes explicit rules on where business logic should reside to ensure architectural consistency.

**Summary:** A comprehensive guide for a complex monorepo that integrates web, mobile, and shared packages. It provides clear operational commands, environment setup, and detailed architectural boundaries.

**Source credibility:** High; a well-maintained open-source productivity platform with significant star count.

**Recency:** 

**Source:** [ever-co/ever-teams/CLAUDE.md](https://github.com/ever-co/ever-teams/blob/335bfe2fd5680fbaf303df111bbd50b729a670ae/CLAUDE.md) · 509★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Ever Teams Project Instructions

This file gives Claude Code (and other AI coding tools) project-specific instructions for working in this repo.

## 1. Project Overview

Ever Teams is an **Open Work and Project Management Platform** built as a monorepo:

- **Web App**: Next.js 16 App Router (`apps/web`) - Main application
- **Mobile App**: React Native (`apps/mobile`)
- **Desktop App**: Electron wrapper (`apps/server-web`)
- **Browser Extensions**: (`apps/extensions`)
- **Shared Packages**: (`packages/*`) - constants, types, services, hooks, utils, ui

## 2. Environment & Tooling

- Always run commands from the **repository root**.
- Node.js: **>= 24.x.x** (see `package.json` engines and `.nvmrc`).
- Primary package manager: **Yarn 1.x** (lockfile: `yarn.lock`).
- Build orchestration: **Turbo** + **Nx** for workspace management.
- Scripts should be invoked via `yarn`; avoid calling `npm` or `pnpm`.

## 3. Install Dependencies

Prefer these commands:

```bash
yarn install
# or
yarn bootstrap
```

- Avoid re-running `yarn install` if `node_modules/` already exists, unless dependencies changed.
- Do **not** add new dependencies without an explicit request; prefer using e
```

</details>
