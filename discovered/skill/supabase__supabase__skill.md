---
name: supabase__supabase__skill
source: https://github.com/supabase/supabase/blob/ebcd052018dfcf1afe282c22e4cb706d4b7e45c5/.claude/skills/studio-testing/SKILL.md
repo: supabase/supabase
kind: skill
stars: 104236
last_pushed: 2026-06-15T09:25:38Z
license: apache-2.0
score: 9
domains: [web-frontend, testing]
tags: [testing-strategy, refactoring, unit-tests]
curated: 2026-06-15
curated_by: config-scout
---

# supabase/supabase — skill

**Why it's worth keeping:** It provides a clear decision tree for selecting test types and highly actionable 'Before vs. After' code examples for refactoring logic out of components.

**Summary:** A high-signal testing strategy that prioritizes extracting business logic from React components into pure, testable utility functions.

**Source credibility:** Extremely high; comes from the Supabase engineering team.

**Recency:** Very current; recently updated and uses modern Vitest/TypeScript standards.

**Source:** [supabase/supabase/.claude/skills/studio-testing/SKILL.md](https://github.com/supabase/supabase/blob/ebcd052018dfcf1afe282c22e4cb706d4b7e45c5/.claude/skills/studio-testing/SKILL.md) · 104236★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: studio-testing
description: Testing strategy for Supabase Studio. Use when writing tests, deciding what
  type of test to write, extracting logic from components into testable utility
  functions, or reviewing test coverage. Covers unit tests, component tests,
  and E2E test selection criteria.
---

# Studio Testing Strategy

How to write and structure tests for `apps/studio/`. The core principle: push
logic out of React components into pure utility functions, then test those
functions exhaustively. Only use component tests for complex UI interactions.
Use E2E tests for features shared between self-hosted and platform.

## When to Apply

Reference these guidelines when:

- Writing new tests for Studio code
- Deciding which type of test to write (unit, component, E2E)
- Extracting logic from a component to make it testable
- Reviewing whether test coverage is sufficient
- Adding a new feature that needs tests

## Rule Categories by Priority

| Priority | Category         | Impact   | Prefix     |
| -------- | ---------------- | -------- | ---------- |
| 1        | Logic Extraction | CRITICAL | `testing-` |
| 2        | Test Coverage    | CRITICAL | `testing-` |
| 3
```

</details>
