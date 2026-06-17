---
name: kyo0221__claude-config__skill-md
source: https://github.com/kyo0221/claude-config/blob/d7d5ec801c07822227c2972f519d9ad68ae11505/skills/tdd/SKILL.MD
repo: kyo0221/claude-config
kind: skill
stars: 0
last_pushed: 2026-05-28T15:12:09Z
license: unknown
score: 9
domains: [software-engineering, testing]
tags: [tdd, workflow, quality-assurance, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# kyo0221/claude-config — skill

**Why it's worth keeping:** The distinction between 'horizontal' and 'vertical' slicing is a powerful guardrail that prevents agents from writing speculative, brittle tests; the 'tracer bullet' concept provides a clear tactical starting point.

**Summary:** Establishes a rigorous TDD framework centered on behavior-driven vertical slices rather than implementation-heavy horizontal blocks.

**Source credibility:** Low repo visibility, but the high density of architectural insight suggests a senior engineer wrote it.

**Recency:** Highly relevant to current agentic workflows that require iterative validation.

**Source:** [kyo0221/claude-config/skills/tdd/SKILL.MD](https://github.com/kyo0221/claude-config/blob/d7d5ec801c07822227c2972f519d9ad68ae11505/skills/tdd/SKILL.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: tdd
description: Test-driven development with red-green-refactor loop. Use when user wants to build features or fix bugs using TDD, mentions "red-green-refactor", wants integration tests, or asks for test-first development.
---

# Test-Driven Development

## Philosophy

**Core principle**: Tests should verify behavior through public interfaces, not implementation details. Code can change entirely; tests shouldn't.

**Good tests** are integration-style: they exercise real code paths through public APIs. They describe _what_ the system does, not _how_ it does it. A good test reads like a specification - "user can checkout with valid cart" tells you exactly what capability exists. These tests survive refactors because they don't care about internal structure.

**Bad tests** are coupled to implementation. They mock internal collaborators, test private methods, or verify through external means (like querying a database directly instead of using the interface). The warning sign: your test breaks when you refactor, but behavior hasn't changed. If you rename an internal function and tests fail, those tests were testing implementation, not behavior.

See [tests.md](tests.md) for e
```

</details>
