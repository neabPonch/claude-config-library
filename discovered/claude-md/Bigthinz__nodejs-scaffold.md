---
name: Bigthinz__nodejs-scaffold
source: https://github.com/Bigthinz/nodejs-scaffold/blob/083cb9809be9f93d7b1368829a9bfc1861af292a/CLAUDE.md
repo: Bigthinz/nodejs-scaffold
kind: claude-md
stars: 0
last_pushed: 2026-05-15T23:11:29Z
license: mit
score: 8
domains: [backend-api, nodejs]
tags: [express, typescript, mongodb, boilerplate, architecture]
curated: 2026-06-14
curated_by: config-scout
---

# Bigthinz/nodejs-scaffold — claude-md

**Why it's worth keeping:** Includes an 'Adding a New Module' workflow which serves as a perfect procedural guide for AI agents, plus detailed pattern documentation to prevent architectural drift.

**Summary:** Defines a clear module-based architecture with explicit instructions for system extension and key implementation details like error handling and path aliasing.

**Source credibility:** Low star count suggests it is likely a personal or niche boilerplate/scaffold.

**Recency:** Up-to-date with modern TypeScript and ESM standards.

**Source:** [Bigthinz/nodejs-scaffold/CLAUDE.md](https://github.com/Bigthinz/nodejs-scaffold/blob/083cb9809be9f93d7b1368829a9bfc1861af292a/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Node Express Scaffold

REST API scaffold built on Node.js + Express + Mongoose + TypeScript. Provides authentication, RBAC, audit logging, notifications, and settings — ready to extend with your domain modules.

## Build & Development Commands

```bash
yarn dev              # Compile TS + start dev server with --watch (NODE_ENV=development)
yarn compile          # Compile TypeScript + resolve aliases + fix ESM imports
yarn start            # Production start via PM2
yarn seed             # Seed permissions, roles, and default settings
yarn test             # Run Jest test suite
yarn lint             # ESLint check
yarn lint:fix         # ESLint fix
yarn prettier         # Prettier check
yarn prettier:fix     # Prettier fix
```

Pre-commit hook runs `lint-staged`. Uses Husky + commitizen with conventional commits.

## Architecture

### Module Structure

All domain logic lives in `src/modules/`. Each module typically contains:
- `*.model.ts` — Mongoose schema/model
- `*.controller.ts` — Express request handlers
- `*.service.ts` — Business logic
- `*.validation.ts` — Joi validation schemas
- `*.interfaces.ts` — TypeScript interfaces
- `*.repository.ts` — Database access
```

</details>
