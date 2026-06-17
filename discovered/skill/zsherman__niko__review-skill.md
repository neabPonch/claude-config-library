---
name: zsherman__niko__review-skill
source: https://github.com/zsherman/niko/blob/af5f699aa5b99238443d5a252a058e7e60dda9f1/.niko/review-skill.md
repo: zsherman/niko
kind: skill
stars: 1
last_pushed: 2026-01-08T16:46:27Z
license: unknown
score: 9
domains: [software-engineering, quality-assurance]
tags: [pr-review, refactoring, anti-laziness]
curated: 2026-06-15
curated_by: config-scout
---

# zsherman/niko — skill

**Why it's worth keeping:** The explicit prohibition of lint/type suppressions and the instruction to favor clean end-states over backward compatibility provide powerful guardrails for agentic coding.

**Summary:** An intensive, 'anti-laziness' code review skill that mandates fixing bugs and refactoring legacy patterns instead of just reporting them.

**Source credibility:** Low star count suggests a niche/experimental tool, but the technical depth indicates high quality.

**Recency:** 5 months old; highly relevant to current agentic workflows.

**Source:** [zsherman/niko/.niko/review-skill.md](https://github.com/zsherman/niko/blob/af5f699aa5b99238443d5a252a058e7e60dda9f1/.niko/review-skill.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Skill: ExhaustiveReview-Style PR Review (Anti-Laziness Edition)

This skill produces a ExhaustiveReview-like pull request review: **top-level PR comment + inline, line-by-line notes**. It emphasizes:

- **High-level summary + technical walkthrough**
- **Line-by-line suggestions (ideally "commit-ready")**
- **Security + quality + missing tests**
- **Fixing issues in place** (not just reporting them)

---

## Non-negotiable policies

### A) No backwards compatibility by default

- Prefer the cleanest end-state.
- If a change breaks callers, **update all call sites** and delete the old API.
- Do not keep adapters/shims unless there is a _hard_ external contract (and if so, explain why).

### B) No silencing the tooling

Disallow "mute the warning" fixes:

- JS/TS: `eslint-disable*`, `@ts-ignore`, `@ts-expect-error`
- Rust: `#[allow(...)]`, `#![allow(...)]`, clippy allowlists
- Python: `# type: ignore`, `# noqa`
- Others: equivalent "ignore" pragmas

If one is truly necessary:

- scope it to the smallest span,
- explain why it's unavoidable,
- include an actionable follow-up (issue link / TODO with plan).

---

## Your task

You are reviewing the changes made in the previous niko ite
```

</details>
