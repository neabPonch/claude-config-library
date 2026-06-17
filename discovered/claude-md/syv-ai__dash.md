---
name: syv-ai__dash
source: https://github.com/syv-ai/dash/blob/3d2de984b10c83aa17d90414f6866742c7d50ff8/CLAUDE.md
repo: syv-ai/dash
kind: claude-md
stars: 276
last_pushed: 2026-06-10T12:30:38Z
license: mit
score: 9
domains: [electron, desktop-app, typescript]
tags: [ipc, architecture, design-system]
curated: 2026-06-15
curated_by: config-scout
---

# syv-ai/dash — claude-md

**Why it's worth keeping:** The explicit mapping of the IPC flow (method → invoke → handler) and specific CSS design token rules are highly transferable patterns for maintaining consistency in complex apps.

**Summary:** Provides a rigorous technical blueprint of an Electron application, detailing IPC communication protocols and data storage paths.

**Source credibility:** Solid open-source project with significant stars and very recent activity.

**Recency:** Highly current, utilizing modern tech like Node 22 and React 18.

**Source:** [syv-ai/dash/CLAUDE.md](https://github.com/syv-ai/dash/blob/3d2de984b10c83aa17d90414f6866742c7d50ff8/CLAUDE.md) · 276★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## What is Dash

Electron desktop app for running Claude Code across multiple projects, each task in its own git worktree. xterm.js + node-pty terminals, SQLite + Drizzle ORM, React 18 UI. macOS arm64, Linux x64.

## Commands

```bash
pnpm install              # install deps
npx electron-rebuild -f -w node-pty,better-sqlite3  # rebuild native modules for Electron
pnpm dev                  # Vite on :3000 + Electron
pnpm dev:main             # main process only
pnpm dev:renderer         # Vite dev server only
pnpm build                # compile main (tsc) + renderer (vite)
pnpm type-check           # typecheck both processes
pnpm package:mac          # build + package as .dmg (arm64)
pnpm package:linux        # build + package as .AppImage (x64)
pnpm drizzle:generate     # generate Drizzle migrations
```

Renderer hot-reloads; main process changes require restart. Husky pre-commit runs lint-staged (Prettier + ESLint on staged `.ts`/`.tsx`).

## Architecture

Two-process Electron app, strict context isolation (nodeIntegration disabled).

- **Main** (`src/main/`): `entry.ts` → `main.ts` boots PATH fix, DB, hook server, IPC handlers, activity monitor, window.
- **Renderer*
```

</details>
