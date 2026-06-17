---
name: nxext__nx-extensions
source: https://github.com/nxext/nx-extensions/blob/9d2b3bfa6e915db4e454923fe9d0e526e8010fec/CLAUDE.md
repo: nxext/nx-extensions
kind: claude-md
stars: 489
last_pushed: 2026-04-20T06:44:24Z
license: mit
score: 9
domains: [monorepo, dev-tools, web-frameworks]
tags: [nx, monorepo, pnpm, typescript, automation]
curated: 2026-06-16
curated_by: config-scout
---

# nxext/nx-extensions — claude-md

**Why it's worth keeping:** It explains two distinct local development workflows (Playground vs. Verdaccio) which prevents the AI from suggesting incorrect setup methods. It also strictly defines architectural constraints like mandatory '@nx/devkit' usage to prevent hand-rolled logic.

**Summary:** This file provides highly detailed context for a complex Nx monorepo, detailing specific commands and sophisticated local testing environments.

**Source credibility:** Highly credible; comes from a well-maintained, popular Nx extension ecosystem with high star counts and regular updates.

**Recency:** Current; uses modern tooling like pnpm, VitePress, and latest Nx patterns.

**Source:** [nxext/nx-extensions/CLAUDE.md](https://github.com/nxext/nx-extensions/blob/9d2b3bfa6e915db4e454923fe9d0e526e8010fec/CLAUDE.md) · 489★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

Nx monorepo that publishes a family of Nx plugins (`@nxext/*`) for non-Angular frameworks: `capacitor`, `ionic-angular`, `ionic-react`, `stencil`, `svelte`, `sveltekit`, `solid`, `preact`, plus a shared `common` library. Plugin majors track the supported Nx major — e.g. `21.x` of a plugin requires Nx `21.x`.

Package manager: **pnpm** (pinned via `packageManager` in root `package.json`). Node version in `.node-version`. Always run `pnpm format` before pushing (enforced in `CONTRIBUTING.md`).

## Workspace layout

`nx.json` overrides the default Nx layout:

- `packages/*` — the publishable plugin libraries (`libsDir`).
- `e2e/*` — the end-to-end test projects (`appsDir`), one per plugin. Each has `implicitDependencies: [<plugin>]`.
- `docs/` — VitePress site (`pnpm start:docs`).
- `tools/scripts/` — playground, local-registry, version-bump, and documentation scripts.
- `tsconfig.base.json` defines `@nxext/*` path aliases that resolve to each package's `src/index.ts`.

Each plugin package follows the standard Nx plugin shape: `generators.json`, `e
```

</details>
