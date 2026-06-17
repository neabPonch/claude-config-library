---
name: dahlia__logtape__skill
source: https://github.com/dahlia/logtape/blob/37602dc668e8a2baa1562ab7938de61bca065c40/.agents/skills/javascript-testing-expert/SKILL.md
repo: dahlia/logtape
kind: skill
stars: 1826
last_pushed: 2026-06-13T13:58:21Z
license: mit
score: 9
domains: [web-frontend, testing, javascript]
tags: [vitest, property-based-testing, tdd, unit-testing]
curated: 2026-06-15
curated_by: config-scout
---

# dahlia/logtape — skill

**Why it's worth keeping:** It provides concrete rules for the AAA pattern, distinguishes between stubs and mocks to prevent brittle tests, and offers advanced strategies for handling non-deterministic values like time and randomness.

**Summary:** An expert-level instruction set for JavaScript testing that prioritizes bug discovery through property-based testing and strict structural patterns. It focuses on Vitest and high-quality unit test architecture.

**Source credibility:** The quality of the instructions reflects highly experienced engineering standards found in popular modern JS libraries.

**Recency:** Very current, incorporating modern tools like Vitest and @fast-check/vitest.

**Source:** [dahlia/logtape/.agents/skills/javascript-testing-expert/SKILL.md](https://github.com/dahlia/logtape/blob/37602dc668e8a2baa1562ab7938de61bca065c40/.agents/skills/javascript-testing-expert/SKILL.md) · 1826★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: javascript-testing-expert
description: Expert-level JavaScript testing skill focused on writing high-quality tests that find bugs, serve as documentation, and prevent regressions. Advocates for property-based testing with fast-check and protects against indeterministic code in tests. Does not cover black-box e2e testing.
---

> **⚠️ Scope:** Testing functions and components, not black-box e2e.

**🏅 Main objectives:** use tests as a way to...

1. uncover hard to detect bugs
2. document how to use the code
3. avoid regressions
4. challenge the code

**🔧 Recommended tooling:** `vitest`, `fast-check`, `@fast-check/vitest`, `@testing-library/*`, `@vitest/browser-playwright`, `msw` installed as devDependencies.  
**✅ Do** try to install missing and relevant tooling, only recommend for `@fast-check/vitest` and browser testing.  
**✅ Do** highly recommend user to install missing and relevant tooling.  
**✅ Do** adapt yourself to missing tools.

## File and code layout

**✅ Do** mimic the existing test structure of the project when adding new tests

**✅ Do** use one test file per code file

**👍 Prefer** using `.spec.ts` extension (e.g., `fileName.ts` → `fileName.spec.ts`) and colo
```

</details>
