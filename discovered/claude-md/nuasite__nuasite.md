---
name: nuasite__nuasite
source: https://github.com/nuasite/nuasite/blob/dfcd98a773578b84f526b6220d443bc537d4b2db/CLAUDE.md
repo: nuasite/nuasite
kind: claude-md
stars: 21
last_pushed: 2026-06-12T15:57:57Z
license: other
score: 9
domains: [web-frontend, cli-tools, monorepo]
tags: [bun, astro, monorepo, cms]
curated: 2026-06-15
curated_by: config-scout
---

# nuasite/nuasite — claude-md

**Why it's worth keeping:** The 'Architecture' section explains non-obvious logic like HTML injection and Vite middleware, while the 'Testing' section lists specific domain-specific helpers to prevent hallucinated test patterns.

**Summary:** Provides high-level architectural mental models for a complex Bun/Astro monorepo and detailed instructions for its custom CMS engine.

**Source credibility:** High technical density despite low star count; reflects a well-structured professional monorepo.

**Recency:** Very current; utilizes modern tooling like Bun, Biome, and Astro.

**Source:** [nuasite/nuasite/CLAUDE.md](https://github.com/nuasite/nuasite/blob/dfcd98a773578b84f526b6220d443bc537d4b2db/CLAUDE.md) · 21★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
# Install dependencies
bun install

# Build all packages (TypeScript declarations + CMS editor bundle)
bun run build

# TypeScript only
bun run ts:build
bun run ts:watch
bun run ts:clean

# Lint (Biome)
bun run lint
bun run lint:fix

# Format (dprint)
bun run format
bun run format:check

# Test (Bun test runner with happy-dom)
bun test
bun test packages/cms/tests/cases/source-finder/search-index.test.ts  # single file
bun test --update-snapshots

# Run a script in a specific package
bun workspace @nuasite/cms run build
```

## Architecture

Bun monorepo with 7 publishable packages under `packages/`, all revolving around the Astro framework:

- **`@nuasite/nua`** — Meta-integration that composes all other integrations into a single `defineConfig()` call.
- **`@nuasite/cms`** — The largest package. Astro integration for inline visual editing. Two core phases:
  1. **HTML processing** — intercepts rendered HTML, parses it with `node-html-parser`, injects `data-cms-id` attributes on editable elements, and generates a per-page manifest (`cms-manifest.
```

</details>
