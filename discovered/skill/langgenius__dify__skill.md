---
name: langgenius__dify__skill
source: https://github.com/langgenius/dify/blob/9b74df21d02b218aa59f4ec7e2600a40f4964192/.agents/skills/frontend-testing/SKILL.md
repo: langgenius/dify
kind: skill
stars: 145285
last_pushed: 2026-06-15T09:26:57Z
license: other
score: 9
domains: [web-frontend, testing]
tags: [vitest, react, rtl, tdd]
curated: 2026-06-15
curated_by: config-scout
---

# langgenius/dify — skill

**Why it's worth keeping:** It mandates a strict 'incremental workflow' (one file at a time) to prevent error accumulation and includes high-level strategy on when to mock vs. use real components.

**Summary:** A highly detailed skill for automating Vitest and React Testing Library suites within the Dify frontend. It provides specific command references, file naming conventions, and mocking strategies.

**Source credibility:** Very high; Dify is a major, highly-starred production-ready open-source platform.

**Recency:** 

**Source:** [langgenius/dify/.agents/skills/frontend-testing/SKILL.md](https://github.com/langgenius/dify/blob/9b74df21d02b218aa59f4ec7e2600a40f4964192/.agents/skills/frontend-testing/SKILL.md) · 145285★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: frontend-testing
description: Generate Vitest + React Testing Library tests for Dify frontend components, hooks, and utilities. Triggers on testing, spec files, coverage, Vitest, RTL, unit tests, integration tests, or write/review test requests.
---

# Dify Frontend Testing Skill

This skill enables Codex to generate high-quality, comprehensive frontend tests for the Dify project following established conventions and best practices.

> **⚠️ Authoritative Source**: This skill is derived from `web/docs/test.md`. Use Vitest mock/timer APIs (`vi.*`).

## When to Apply This Skill

Apply this skill when the user:

- Asks to **write tests** for a component, hook, or utility
- Asks to **review existing tests** for completeness
- Mentions **Vitest**, **React Testing Library**, **RTL**, or **spec files**
- Requests **test coverage** improvement
- Uses `pnpm analyze-component` output as context
- Mentions **testing**, **unit tests**, or **integration tests** for frontend code
- Wants to understand **testing patterns** in the Dify codebase

**Do NOT apply** when:

- User is asking about backend/API tests (Python/pytest)
- User is asking about E2E tests (Cucumber + Playwright under `e
```

</details>
