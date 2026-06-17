---
name: stagewise-io__stagewise
source: https://github.com/stagewise-io/stagewise/blob/9f11e7c585183016273dcd1d47c9aeaee8014850/CLAUDE.md
repo: stagewise-io/stagewise
kind: claude-md
stars: 6681
last_pushed: 2026-06-15T17:49:29Z
license: agpl-3.0
score: 9
domains: [monorepo, web-frontend, desktop-app, cli-tools]
tags: [pnpm, turborepo, electron, typescript]
curated: 2026-06-16
curated_by: config-scout
---

# stagewise-io/stagewise — claude-md

**Why it's worth keeping:** It uses explicit tool-chain warnings (e.g., Biome vs ESLint) and defines precise commit scope patterns that are highly transferable to any large-scale workspace.

**Summary:** Provides comprehensive command groupings, architecture maps, and strict contribution standards for a complex pnpm monorepo.

**Source credibility:** Highly credible source with 6k+ stars and recent activity.

**Recency:** Very current, referencing modern technologies like React 19 and Tailwind 4.

**Source:** [stagewise-io/stagewise/CLAUDE.md](https://github.com/stagewise-io/stagewise/blob/9f11e7c585183016273dcd1d47c9aeaee8014850/CLAUDE.md) · 6681★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Essential Commands

### Development
- `pnpm install` - Install dependencies (Node >= 18, pnpm 10.x required)
- `pnpm dev` - Start all packages in watch mode (Turbo watch across workspaces)
- `pnpm dev:examples` - Watch mode for example applications
- `pnpm dev:plugins` - Watch mode for plugin packages

### Building
- `pnpm build` - Build all packages and apps
- `pnpm build:apps` - Build applications only (`apps/*`)
- `pnpm build:packages` - Build packages only (`packages/*`)
- `pnpm build:toolbar` - Build toolbar packages (`toolbar/*`)
- `pnpm build:plugins` - Build plugin packages (`plugins/*`)

### Code Quality
- `pnpm check` - Run Biome linting/formatting checks (read-only)
- `pnpm check:fix` - Auto-fix linting/formatting issues
- `pnpm typecheck` - Run TypeScript type checking across monorepo

### Testing
- `pnpm test` - Run tests via Vitest across workspaces
- `pnpm -F <package-name> test` - Run tests for specific package (e.g., `pnpm -F @stagewise/karton test`)

### Browser App Specific
- `pnpm -F stagewise start` - Start the Electron browser app (with typec
```

</details>
