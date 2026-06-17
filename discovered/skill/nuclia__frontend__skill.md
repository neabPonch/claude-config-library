---
name: nuclia__frontend__skill
source: https://github.com/nuclia/frontend/blob/a62cc932767fb74326917e56a4537ac2c4b6b87e/.claude/skills/rxjs-patterns/SKILL.md
repo: nuclia/frontend
kind: skill
stars: 56
last_pushed: 2026-06-15T17:39:18Z
license: mit
score: 9
domains: [web-frontend, angular, rxjs]
tags: [rx-js, angular, patterns, state-management]
curated: 2026-06-15
curated_by: config-scout
---

# nuclia/frontend — skill

**Why it's worth keeping:** Provides practical decision matrices for operator selection and specific 'non-negotiable' rules that prevent common memory leaks and stream completion bugs. The comparison between ReplaySubject(1) and BehaviorSubject for avoiding null-sentinels is a highly transferable senior-level pattern.

**Summary:** Encodes high-level RxJS and Angular architecture decisions used in a production monorepo to ensure stream stability and state consistency.

**Source credibility:** High; sourced from an active, real-world RAG-as-a-Service frontend repository.

**Recency:** Very current; includes modern Angular patterns like Signals and `takeUntilDestroyed()`.

**Source:** [nuclia/frontend/.claude/skills/rxjs-patterns/SKILL.md](https://github.com/nuclia/frontend/blob/a62cc932767fb74326917e56a4537ac2c4b6b87e/.claude/skills/rxjs-patterns/SKILL.md) · 56★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: rxjs-patterns
description: >
  RxJS patterns as used in the Nuclia frontend monorepo — covering Subject type selection,
  flattening operator decisions (switchMap vs concatMap vs mergeMap), combination operators
  (combineLatest vs forkJoin vs withLatestFrom), error handling, shareReplay placement,
  cleanup strategies, debounce conventions, Angular signal interop, and import hygiene.
  Activate this skill for ANY task that touches observable pipelines, service state streams,
  RxJS subscriptions, or operator choices in Angular apps or libs. Do not wait to be asked
  about "RxJS patterns" specifically — if the task writes or modifies a .pipe(), creates a
  Subject, adds a subscription in a service or component, uses catchError/switchMap/forkJoin,
  or asks "which operator should I use here?", this skill applies. Also use when debugging
  streams that never emit, emit multiple times unexpectedly, or cause memory leaks. This skill
  covers Angular libs and apps only; it does not cover search-widget (Svelte) or rao-widget (React).
---

# RxJS Patterns — Nuclia Frontend Monorepo

This skill encodes patterns as they are **actually used** in this codebase. RxJS has hundreds of
```

</details>
