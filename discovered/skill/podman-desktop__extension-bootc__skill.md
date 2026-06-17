---
name: podman-desktop__extension-bootc__skill
source: https://github.com/podman-desktop/extension-bootc/blob/cdb90252746825f8fe4cc98eea370a4d39b93345/.agents/skills/unit-testing/SKILL.md
repo: podman-desktop/extension-bootc
kind: skill
stars: 476
last_pushed: 2026-06-15T02:42:28Z
license: apache-2.0
score: 9
domains: [web-frontend, backend-api, testing]
tags: [vitest, svelte, monorepo, unit-testing]
curated: 2026-06-15
curated_by: config-scout
---

# podman-desktop/extension-bootc — skill

**Why it's worth keeping:** Includes explicit 'discovery' commands (grep) to help the agent learn existing mock patterns by observing current codebase implementations and provides specific pnpm workflows for all package layers.

**Summary:** Provides comprehensive unit testing instructions for a multi-package monorepo, covering Node.js backend, Svelte frontend, and shared logic using Vitest.

**Source credibility:** High; part of an active, well-maintained Podman Desktop extension.

**Recency:** Highly current, referencing modern tooling like Vitest 4 and pnpm.

**Source:** [podman-desktop/extension-bootc/.agents/skills/unit-testing/SKILL.md](https://github.com/podman-desktop/extension-bootc/blob/cdb90252746825f8fe4cc98eea370a4d39b93345/.agents/skills/unit-testing/SKILL.md) · 476★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: unit-testing
description: >-
  Guides writing and maintaining Vitest unit tests for the bootc extension's
  backend, frontend, and shared packages. Covers mocking @podman-desktop/api,
  RPC clients, Svelte stores, and Node.js modules. Triggers when creating or
  modifying .spec.ts files, fixing Vitest failures, or adding test coverage.
paths:
  - packages/backend/src/**/*.spec.ts
  - packages/frontend/src/**/*.spec.ts
  - packages/shared/src/**/*.spec.ts
argument-hint: '[test-file-or-pattern]'
---

# Unit Testing for Bootc Extension

## Framework

- **Vitest 4** with v8 coverage provider
- **Backend**: Node.js environment, mocked `@podman-desktop/api`
- **Frontend**: JSDOM environment, `@testing-library/svelte` for components
- **Shared**: Node.js environment for message proxy and model tests

## Running Tests

```bash
pnpm test              # all packages
pnpm test:backend      # packages/backend with coverage
pnpm test:frontend     # packages/frontend with coverage
pnpm test:shared       # packages/shared with coverage

# Single file
npx vitest run packages/backend/src/build-disk-image.spec.ts

# Watch mode
npx vitest watch packages/backend/src/
```

## Backend Test Pat
```

</details>
