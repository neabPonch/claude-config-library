---
name: stormasm__nunotes__piet-skill
source: https://github.com/stormasm/nunotes/blob/482ec2f003aec575cdf962c5b5ae6e3358471aa4/ai/piet-skill.md
repo: stormasm/nunotes
kind: skill
stars: 11
last_pushed: 2026-06-12T14:32:58Z
license: mit
score: 8
domains: [cli-tools, rust, testing]
tags: [refactoring, migration, integration-tests]
curated: 2026-06-14
curated_by: config-scout
---

# stormasm/nunotes — skill

**Why it's worth keeping:** It demonstrates the 'ground truth' technique: instructing the agent to inspect specific source files as API references rather than relying on internal knowledge, and provides strict safety rules to prevent assertion degradation.

**Summary:** A highly specific migration skill for updating Nushell integration tests from a deprecated macro to a new test harness.

**Source credibility:** Low-star/niche repository that appears to be a specialized tool for active Nushell contributors.

**Recency:** Current; utilizes modern 'inspect-then-edit' workflows essential for high-stakes refactoring.

**Source:** [stormasm/nunotes/ai/piet-skill.md](https://github.com/stormasm/nunotes/blob/482ec2f003aec575cdf962c5b5ae6e3358471aa4/ai/piet-skill.md) · 11★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: nushell-test-refactor
description: Refactor Nushell integration tests from deprecated nu_test_support::nu! usage to nu_test_support::test() with the right prelude imports and migration patterns
license: MIT
compatibility: opencode
metadata:
  audience: nushell-contributors
  workflow: refactoring
  language: rust
---

# Skill: nushell-test-refactor

Refactor Nushell integration tests away from deprecated `nu_test_support::nu!` calls and toward `nu_test_support::test()` usage.

## When to use this skill

Use this skill when you are updating Nushell integration tests that still use `nu_test_support::nu!`, especially when:

- tests are being migrated to the newer test harness
- imports need to be normalized around `nu_test_support::prelude::*`
- many files need the same refactor pattern
- you have example refactors, a git diff, or known-good migrated files to follow

Do not use this skill for unrelated Rust refactors or for unit tests that do not depend on the Nushell test support helpers.

## Core migration rule

Prefer `nu_test_support::test()` over `nu_test_support::nu!` for integration tests.

Use `nu_test_support::prelude::*` as the starting import when possible, since
```

</details>
