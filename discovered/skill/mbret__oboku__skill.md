---
name: mbret__oboku__skill
source: https://github.com/mbret/oboku/blob/145a9cb33266761d3a2599352362e40e083a5179/.agents/skills/rxjs-like-a-pro/SKILL.md
repo: mbret/oboku
kind: skill
stars: 29
last_pushed: 2026-06-01T11:50:01Z
license: gpl-3.0
score: 9
domains: [web-frontend, reactive-programming]
tags: [rxjs, typescript, observables, patterns]
curated: 2026-06-15
curated_by: config-scout
---

# mbret/oboku — skill

**Why it's worth keeping:** Includes specific 'Bad vs Good' examples for flattening operators, error handling placement, and memory leak prevention via takeUntil logic.

**Summary:** Establishes a high-standard mental model for writing idiomatic RxJS by prioritizing declarative pipelines over imperative subscriptions.

**Source credibility:** High-quality technical depth despite the relatively small repository size.

**Recency:** Highly relevant to modern reactive programming standards used in current frontend development.

**Source:** [mbret/oboku/.agents/skills/rxjs-like-a-pro/SKILL.md](https://github.com/mbret/oboku/blob/145a9cb33266761d3a2599352362e40e083a5179/.agents/skills/rxjs-like-a-pro/SKILL.md) · 29★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: rxjs-like-a-pro
description: >
  How to write idiomatic, efficient RxJS code. Use this skill whenever the user is writing, refactoring,
  reviewing, or debugging code that uses RxJS — including any file that imports from 'rxjs' or 'rxjs/operators'.
  Trigger on mentions of observables, subscriptions, RxJS operators, or reactive streams. Even if the user
  doesn't say "RxJS" explicitly, activate when you see patterns like `.pipe()`, `.subscribe()`, `Observable`,
  `Subject`, `BehaviorSubject`, `switchMap`, `mergeMap`, or similar.
---

# RxJS Like a Pro

This skill helps you write RxJS code that is idiomatic, composable, and free of common pitfalls. The core
philosophy: **keep logic in the observable chain**. Every time you reach for `.subscribe()`, ask whether the
work could instead be expressed as a transformation inside `.pipe()`.

## Reference files

For detailed examples and patterns, read the relevant reference file:

- `references/loading-state-patterns.md` — Deriving loading/error state in the chain, the `withLoadingState`
  custom operator, and using `scan` to preserve previous results across loading states. Read when working with
  async data fetching that needs l
```

</details>
