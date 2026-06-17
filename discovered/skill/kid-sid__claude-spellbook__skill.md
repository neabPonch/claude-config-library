---
name: kid-sid__claude-spellbook__skill
source: https://github.com/kid-sid/claude-spellbook/blob/a51ebdd8902ca9b8d3b9c6569c415bdb280e6e34/skills/solution-testing/skill.md
repo: kid-sid/claude-spellbook
kind: skill
stars: 175
last_pushed: 2026-06-02T19:47:52Z
license: mit
score: 9
domains: [web-frontend, testing, automation]
tags: [playwright, e2e, tdd, bdd]
curated: 2026-06-16
curated_by: config-scout
---

# kid-sid/claude-spellbook — skill

**Why it's worth keeping:** The 'Bad vs Good' code comparisons and the Locator Strategy priority table are excellent guardrails that prevent an AI from writing fragile or non-semantic test code.

**Summary:** Provides highly opinionated standards for end-to-end testing using Playwright, emphasizing the Page Object Model and semantic locators.

**Source credibility:** High; part of a highly-starred, actively maintained specialized repository.

**Recency:** Current; uses modern Playwright patterns and TypeScript standards.

**Source:** [kid-sid/claude-spellbook/skills/solution-testing/skill.md](https://github.com/kid-sid/claude-spellbook/blob/a51ebdd8902ca9b8d3b9c6569c415bdb280e6e34/skills/solution-testing/skill.md) · 175★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: solution-testing
description: Use when writing Playwright E2E tests for critical user journeys, setting up post-deployment smoke tests, debugging flaky browser automation, or implementing BDD feature files with Gherkin.
---

# Solution Testing

End-to-end and acceptance testing techniques for verifying that a feature works correctly across the full stack — browser, API, and data layer — from the user's perspective.

## When to Activate

- Writing browser automation tests for user journeys
- Verifying a full feature works end-to-end (UI through DB)
- Setting up Playwright or Cypress for a project
- Writing BDD feature files with Gherkin syntax
- Designing smoke tests for post-deployment verification
- Debugging flaky E2E tests
- Deciding how many E2E tests to write for a feature

## E2E vs Integration: The Boundary

E2E tests cover things integration tests cannot:

- Real browser rendering and JavaScript execution (layout, event handling, hydration)
- Full stack traversal: UI → API → DB → UI response cycle
- Multi-step user journeys across pages, sessions, and auth boundaries

### Cost of Each Test Level

| Type        | Speed         | Flakiness Risk | Maintenance Cost |
```

</details>
