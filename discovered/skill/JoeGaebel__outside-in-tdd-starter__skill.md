---
name: JoeGaebel__outside-in-tdd-starter__skill
source: https://github.com/JoeGaebel/outside-in-tdd-starter/blob/9f25776b04ae59f266139ed2a3b983d5f1b73387/.claude/skills/cypress-end-to-end-testing/skill.md
repo: JoeGaebel/outside-in-tdd-starter
kind: skill
stars: 26
last_pushed: 2026-03-10T01:22:42Z
license: unknown
score: 9
domains: [web-frontend, testing, tdd]
tags: [cypress, e2e, tdd, testing-automation]
curated: 2026-06-15
curated_by: config-scout
---

# JoeGaebel/outside-in-tdd-starter — skill

**Why it's worth keeping:** Includes a brilliant 'Right vs. Wrong Failure' diagnostic framework to prevent agent loops and provides specific instructions on extending existing test flows to maintain state consistency.

**Summary:** Defines a rigorous Outside-In TDD workflow for Cypress E2E testing, distinguishing between business process and infrastructure tests.

**Source credibility:** High-quality specialized TDD starter kit with recent maintenance.

**Recency:** Extremely current, specifically tailored for modern agentic coding workflows.

**Source:** [JoeGaebel/outside-in-tdd-starter/.claude/skills/cypress-end-to-end-testing/skill.md](https://github.com/JoeGaebel/outside-in-tdd-starter/blob/9f25776b04ae59f266139ed2a3b983d5f1b73387/.claude/skills/cypress-end-to-end-testing/skill.md) · 26★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cypress-end-to-end-testing
description: Write Cypress end-to-end tests for business processes and cross-cutting infrastructure. Use for testing complete business workflows, authentication flows, and UI state verification.
---

# Cypress End-to-End Testing

Write end-to-end tests organized as **business process tests** or **infrastructure tests**. Business process tests prove a complete business process achieves its outcome. Infrastructure tests verify cross-cutting concerns (auth, security) that don't belong to a specific business process.

## Inputs

See `.claude/agents/tdd-test-writer-contract.md` — "e2e" section for field definitions.

## Write Complete Tests Upfront

Write ALL assertions for the complete feature flow at once. The test should fail because NOTHING is implemented yet, not because one piece is missing. This gives a complete definition of "done" before any implementation begins.

Include all:
- Content the user sees (text, labels, data values — NOT CSS classes or DOM structure)
- User interactions (clicks, inputs, form submissions)
- Expected outcomes (navigation, data changes, confirmation messages)
- Error handling if applicable

## How to Write the Test
```

</details>
