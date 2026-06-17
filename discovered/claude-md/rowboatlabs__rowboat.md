---
name: rowboatlabs__rowboat
source: https://github.com/rowboatlabs/rowboat/blob/e2178c148871ed8ebe6bc3106471f5c2b09cddb6/CLAUDE.md
repo: rowboatlabs/rowboat
kind: claude-md
stars: 14973
last_pushed: 2026-06-15T16:29:40Z
license: apache-2.0
score: 9
domains: [desktop-app, monorepo, fullstack]
tags: [electron, monorepo, build-system, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# rowboatlabs/rowboat — claude-md

**Why it's worth keeping:** It explains the 'why' behind the architecture (e.g., esbuild vs symlinks) and provides precise CLI command paths to prevent navigation errors in nested workspaces.

**Summary:** A highly detailed guide for a complex monorepo involving Electron and Next.js, focusing on build orders and specific entry points.

**Source credibility:** High; a popular, actively maintained repository with significant star count.

**Recency:** Very current, utilizing latest tech versions like React 19 and Electron 39.

**Source:** [rowboatlabs/rowboat/CLAUDE.md](https://github.com/rowboatlabs/rowboat/blob/e2178c148871ed8ebe6bc3106471f5c2b09cddb6/CLAUDE.md) · 14973★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - AI Coding Agent Context

This file provides context for AI coding agents working on the Rowboat monorepo.

## Quick Reference Commands

```bash
# Electron App (apps/x)
cd apps/x && pnpm install          # Install dependencies
cd apps/x && npm run deps          # Build workspace packages (shared → core → preload)
cd apps/x && npm run dev           # Development mode (builds deps, runs app)
cd apps/x && npm run lint          # Lint check
cd apps/x/apps/main && npm run package   # Production build (.app)
cd apps/x/apps/main && npm run make      # Create DMG distributable
```

## Monorepo Structure

```
rowboat/
├── apps/
│   ├── x/                 # Electron desktop app (focus of this doc)
│   ├── rowboat/           # Next.js web dashboard
│   ├── rowboatx/          # Next.js frontend
│   ├── cli/               # CLI tool
│   ├── python-sdk/        # Python SDK
│   └── docs/              # Documentation site
├── CLAUDE.md              # This file
└── README.md              # User-facing readme
```

## Electron App Architecture (`apps/x`)

The Electron app is a **nested pnpm workspace** with its own package management.

```
apps/x/
├── package.json           # Workspace r
```

</details>
