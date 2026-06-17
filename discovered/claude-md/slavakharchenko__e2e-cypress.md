---
name: slavakharchenko__e2e-cypress
source: https://github.com/slavakharchenko/e2e-cypress/blob/88a474e0db328eae448ff28af908e6eb5b5c553c/CLAUDE.md
repo: slavakharchenko/e2e-cypress
kind: claude-md
stars: 1
last_pushed: 2026-03-27T14:00:51Z
license: unknown
score: 9
domains: [web-frontend, e2e-testing, automation]
tags: [cypress, typescript, pom, testing-template]
curated: 2026-06-15
curated_by: config-scout
---

# slavakharchenko/e2e-cypress — claude-md

**Why it's worth keeping:** It defines concrete architectural constraints like the 'Three-Layer Pattern' and selector priority, ensuring Claude generates stable, non-brittle test code. The inclusion of TypeScript examples showing method chaining (returning 'this') is an excellent way to enforce pattern consistency.

**Summary:** A highly structured instruction set for building Cypress E2E test suites using a strict three-layer Page Object Model architecture.

**Source credibility:** Single star repository, but the content reflects professional-grade testing architecture.

**Recency:** Current; follows modern Cypress and TypeScript best practices.

**Source:** [slavakharchenko/e2e-cypress/CLAUDE.md](https://github.com/slavakharchenko/e2e-cypress/blob/88a474e0db328eae448ff28af908e6eb5b5c553c/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Cypress E2E Test Template

## File Sync Rule

**README.md and CLAUDE.md must stay in sync.** README.md is a shortened version of CLAUDE.md (no code examples, condensed rules). When you update either file, update the other to match:

- CLAUDE.md updated → update README.md (condense new content)
- README.md updated → update CLAUDE.md (expand with full details/examples)

## Project Overview

This is a Cypress E2E testing template using TypeScript, Page Object Model (POM), and reusable Page Element components. The architecture separates selectors, actions, and assertions into composable layers.

## Commands

- `npm run cy:open` — open Cypress Test Runner (interactive)
- `npm run cy:run` — run tests headlessly
- `npm run lint` — check ESLint
- `npm run lint:fix` — auto-fix ESLint issues
- `npm run format` — format with Prettier
- `npm run format:check` — check formatting

## Architecture

```
cypress/
├── api/                  # API client classes (BaseApi subclasses)
├── db/                   # Database client (Knex.js) and task functions
├── e2e/                  # Test specs (*.cy.ts)
├── page-elements/        # Reusable UI element classes
├── page-objects/         # Pa
```

</details>
