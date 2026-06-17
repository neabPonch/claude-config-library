---
name: localazy__strapi-plugin
source: https://github.com/localazy/strapi-plugin/blob/c5f4ed531c9a0b4f86bf24cf50270376ba06f8b4/CLAUDE.md
repo: localazy/strapi-plugin
kind: claude-md
stars: 21
last_pushed: 2026-05-15T14:43:26Z
license: mit
score: 8
domains: [backend-api, web-frontend, cms-plugin]
tags: [architecture-map, command-reference]
curated: 2026-06-15
curated_by: config-scout
---

# localazy/strapi-plugin — claude-md

**Why it's worth keeping:** The hierarchical directory breakdown and the specific single-file test execution pattern are highly transferable techniques for large repositories.

**Summary:** Provides a detailed architectural map of both server-side (Node/CommonJS) and admin-side (React) logic, along with specific CLI commands.

**Source credibility:** High; this is an official plugin from a specialized localization company with active maintenance.

**Recency:** Current; it references modern technologies like Strapi v5, Vite, and ESLint flat config.

**Source:** [localazy/strapi-plugin/CLAUDE.md](https://github.com/localazy/strapi-plugin/blob/c5f4ed531c9a0b4f86bf24cf50270376ba06f8b4/CLAUDE.md) · 21★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is `@localazy/strapi-plugin` — the official Strapi v5 plugin by Localazy for managing multilingual content. It connects a Strapi CMS instance to the Localazy localization platform, enabling upload/download of translatable content.

## Commands

```bash
npm run build              # Build the plugin (uses strapi-plugin CLI)
npm run lint               # ESLint (flat config, eslint.config.mjs)
npm run lint:fix           # ESLint with auto-fix
npm run format:check       # Prettier check
npm run format             # Prettier write
npm run test:server        # Run server-side Jest tests
npm run test:server:watch  # Jest in watch mode
npm run test:server:coverage  # Jest with coverage
npm run verify             # Strapi plugin verification
```

Run a single test file:

```bash
npx jest --config server/jest.config.ts server/src/utils/__tests__/<file>.test.ts
```

Node version: specified in `.nvmrc` (currently 20).

## Architecture

The plugin follows the standard Strapi v5 plugin structure with two main entry points:

### `server/src/` — Backend (Nod
```

</details>
