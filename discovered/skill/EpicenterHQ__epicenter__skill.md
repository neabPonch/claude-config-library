---
name: EpicenterHQ__epicenter__skill
source: https://github.com/EpicenterHQ/epicenter/blob/2e955d0e6e1cea75ebf1e536e9e35357e67e84a5/.agents/skills/testing/SKILL.md
repo: EpicenterHQ/epicenter
kind: skill
stars: 4625
last_pushed: 2026-06-15T01:17:19Z
license: other
score: 9
domains: [typescript, testing, software-architecture]
tags: [test-standards, documentation, naming-conventions]
curated: 2026-06-15
curated_by: config-scout
---

# EpicenterHQ/epicenter — skill

**Why it's worth keeping:** The {action} {outcome} [condition] naming pattern and the explicit distinction between behavior tests (*.test.ts) and benchmarks (*.bench.ts) are elite-tier developer habits.

**Summary:** Provides highly opinionated, rigorous standards for test structure, documentation, naming conventions, and file organization.

**Source credibility:** High; from EpicenterHQ, a high-star, active open-source project.

**Recency:** Very current; utilizes modern tooling like Bun and follows contemporary TypeScript testing best practices.

**Source:** [EpicenterHQ/epicenter/.agents/skills/testing/SKILL.md](https://github.com/EpicenterHQ/epicenter/blob/2e955d0e6e1cea75ebf1e536e9e35357e67e84a5/.agents/skills/testing/SKILL.md) · 4625★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: testing
description: 'Test file conventions: setup functions, factories, organization, type testing, naming, and pruning low-value tests. Use when: "write tests", "add a test", "fix this test", "delete tests", "prune tests", "audit tests", or modifying *.test.ts files.'
metadata:
  author: epicenter
  version: '2.0'
---

# Test File Conventions

## When to Apply This Skill

Use this pattern when you need to:

- Write or refactor `*.test.ts` files in this codebase.
- Structure tests with `setup()` functions instead of mutable `beforeEach` setup.
- Split large test files into focused behavior/type/scenario files.
- Enforce behavior-based test naming and clear failure intent.
- Add or review negative type tests using `@ts-expect-error`.
- Audit a test file for assertions that cannot fail or fakes that don't earn their lines.
- Prune tests that cannot name a real regression they would catch.

## References

Load these on demand based on what you're working on:

- If working with **negative type tests** (`@ts-expect-error`, `bun:test` type strategy, no `as any`), read [references/type-testing.md](references/type-testing.md)
- If working with **test setup architecture** (`setup
```

</details>
