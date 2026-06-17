---
name: dahlia__optique__skill
source: https://github.com/dahlia/optique/blob/9eae556a5e51a6904ba3560bc99579d5b59d8a43/.agents/skills/javascript-testing-expert/SKILL.md
repo: dahlia/optique
kind: skill
stars: 699
last_pushed: 2026-06-13T11:45:06Z
license: mit
score: 9
domains: [testing, javascript, typescript]
tags: [tdd, property-based-testing, unit-tests]
curated: 2026-06-15
curated_by: config-scout
---

# dahlia/optique — skill

**Why it's worth keeping:** It teaches the agent to avoid non-determinism by injecting dependencies like dates and distinguishes between example-based and property-based testing for better edge-case coverage.

**Summary:** Provides a sophisticated testing philosophy focused on high-quality unit tests and property-based testing using fast-check.

**Source credibility:** High; derived from a legitimate, well-starred TypeScript CLI library (Optique).

**Recency:** Current; utilizes modern Node.js built-in test runner patterns.

**Source:** [dahlia/optique/.agents/skills/javascript-testing-expert/SKILL.md](https://github.com/dahlia/optique/blob/9eae556a5e51a6904ba3560bc99579d5b59d8a43/.agents/skills/javascript-testing-expert/SKILL.md) · 699★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: javascript-testing-expert
description: Expert-level JavaScript testing skill focused on writing high-quality tests that find bugs, serve as documentation, and prevent regressions. Advocates for property-based testing with fast-check and protects against indeterministic code in tests. Does not cover black-box e2e testing.
---

# JavaScript testing expert

> **⚠️ Scope:** Testing functions and components, not black-box e2e.

**🏅 Main objectives:** use tests as a way to...

1. uncover hard to detect bugs
2. document how to use the code
3. avoid regressions
4. challenge the code

**🔧 Recommended tooling for Optique:** `node:test`, `node:assert/strict`, and `fast-check`.
**✅ Do** try to install only missing and relevant tooling.
**✅ Do** recommend Node's built-in test libraries for Optique tests.
**✅ Do** adapt yourself to missing tools.

## File and code layout

**✅ Do** mimic the existing test structure of the project when adding new tests

**✅ Do** use one test file per code file

**👍 Prefer** using `.test.ts` extension (e.g., `fileName.ts` → `fileName.test.ts`) and colocating tests with the source file, matching the project's existing examples

**✅ Do** put `it` within `de
```

</details>
