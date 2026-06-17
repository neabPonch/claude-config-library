---
name: safe-global__safe-wallet-monorepo__skill
source: https://github.com/safe-global/safe-wallet-monorepo/blob/00c0949f977ea650a9af6d51c81ef60a306541ad/.claude/skills/cypress-e2e/SKILL.md
repo: safe-global/safe-wallet-monorepo
kind: skill
stars: 575
last_pushed: 2026-06-15T18:02:28Z
license: gpl-3.0
score: 9
domains: [web-frontend, e2e-testing, quality-assurance]
tags: [cypress, page-object-model, automation, testing-patterns]
curated: 2026-06-16
curated_by: config-scout
---

# safe-global/safe-wallet-monorepo — skill

**Why it's worth keeping:** It includes specific anti-flakiness techniques, such as mandating that action functions wait for UI settlement, and defines a strict structural pattern for composite flows.

**Summary:** Provides highly structured instructions for Cypress E2E automation using the Page Object Model with rigorous standards for selectors and actions.

**Source credibility:** High; comes from the Safe{Wallet} repository, a prominent and well-maintained smart account project.

**Recency:** Current; utilizes modern testing best practices like data-testid emphasis and semantic HTML targeting.

**Source:** [safe-global/safe-wallet-monorepo/.claude/skills/cypress-e2e/SKILL.md](https://github.com/safe-global/safe-wallet-monorepo/blob/00c0949f977ea650a9af6d51c81ef60a306541ad/.claude/skills/cypress-e2e/SKILL.md) · 575★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cypress-e2e
description: Write or refactor Cypress E2E tests following Page Object Model, action/assertion separation, and project conventions. Use when creating new tests, refactoring existing ones, or adding page object functions.
argument-hint: '[test-description-or-file-path]'
allowed-tools:
  - Read
  - Edit
  - Write
  - Bash
  - Grep
  - Glob
  - Agent
---

# Cypress E2E Test Automation

Write or refactor Cypress E2E tests for **$ARGUMENTS**.

Read `apps/web/cypress/CLAUDE.md` and `apps/web/cypress/AGENTS.md` for project-specific conventions before proceeding.

## Phase 1: Understand Context

1. Read the relevant test file(s) and page object(s) in `apps/web/cypress/e2e/pages/`
2. Read `apps/web/cypress/CLAUDE.md` for conventions
3. Identify which page object file to use (or create)
4. Check existing functions in ALL `*.page*.js` files and `main.page.js` before creating anything new
5. Check the actual React component DOM to understand what `data-testid` attributes exist and which component renders them

## Phase 2: Page Object Structure

Organize page object files in clear sections with this order:

```js
// 1. Imports
// 2. Selectors — grouped by feature area, wit
```

</details>
