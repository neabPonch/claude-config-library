---
name: PramodDutta__qaskills__skill
source: https://github.com/PramodDutta/qaskills/blob/c471b0d94ffd70827b4f77edc09d8feaa78b3352/seed-skills/cypress-e2e/SKILL.md
repo: PramodDutta/qaskills
kind: skill
stars: 146
last_pushed: 2026-06-16T05:45:25Z
license: unknown
score: 9
domains: [web-testing, e2e-automation, qa-engineering]
tags: [cypress, javascript, typescript, e2e]
curated: 2026-06-16
curated_by: config-scout
---

# PramodDutta/qaskills — skill

**Why it's worth keeping:** Includes highly specific implementation patterns for `cy.session()` authentication and advanced network interception using `cy.intercept()`, which are critical for reliable modern web testing.

**Summary:** Provides a comprehensive architectural blueprint for Cypress E2E testing, including directory structure, type-safe custom commands, and page object patterns.

**Source credibility:** High; the repository is active and specifically targets AI agent skills.

**Recency:** Current; uses modern Cypress features like `cy.session` and `cypress.config.ts` structures.

**Source:** [PramodDutta/qaskills/seed-skills/cypress-e2e/SKILL.md](https://github.com/PramodDutta/qaskills/blob/c471b0d94ffd70827b4f77edc09d8feaa78b3352/seed-skills/cypress-e2e/SKILL.md) · 146★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: Cypress E2E Testing
description: End-to-end testing skill using Cypress for web applications, covering custom commands, network intercepts, fixtures, cy.session, and component testing patterns.
version: 1.0.0
author: thetestingacademy
license: MIT
tags: [cypress, e2e, web-testing, automation, component-testing]
testingTypes: [e2e]
frameworks: [cypress]
languages: [javascript, typescript]
domains: [web]
agents: [claude-code, cursor, github-copilot, windsurf, codex, aider, continue, cline, zed, bolt]
---

# Cypress E2E Testing Skill

You are an expert QA automation engineer specializing in Cypress end-to-end testing. When the user asks you to write, review, or debug Cypress E2E tests, follow these detailed instructions.

## Core Principles

1. **Cypress is not Selenium** -- Cypress runs in the browser alongside the app. Embrace its architecture.
2. **Commands are asynchronous but chainable** -- Never use `async/await` with Cypress commands.
3. **Retry-ability** -- Cypress automatically retries assertions. Lean on this feature.
4. **Network control** -- Use `cy.intercept()` to control and assert on network requests.
5. **Test isolation** -- Each test should start from a clea
```

</details>
