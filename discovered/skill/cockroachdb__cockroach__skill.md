---
name: cockroachdb__cockroach__skill
source: https://github.com/cockroachdb/cockroach/blob/f0bf32430c4960bfdad6d867e6df0e67079aeee1/pkg/ui/.claude/skills/redux-to-swr/SKILL.md
repo: cockroachdb/cockroach
kind: skill
stars: 32206
last_pushed: 2026-06-11T22:40:23Z
license: other
score: 9
domains: [web-frontend, refactoring]
tags: [redux, swr, react, migration-guide]
curated: 2026-06-15
curated_by: config-scout
---

# cockroachdb/cockroach — skill

**Why it's worth keeping:** It provides specific implementation patterns for complex scenarios like conditional fetching and key design, while explicitly defining anti-patterns to avoid during refactoring.

**Summary:** A highly detailed technical blueprint for migrating legacy Redux/Saga state management to modern SWR-based data fetching in React.

**Source credibility:** Extremely high; sourced from the highly-starred CockroachDB production repository.

**Recency:** Very current; the source is actively maintained.

**Source:** [cockroachdb/cockroach/pkg/ui/.claude/skills/redux-to-swr/SKILL.md](https://github.com/cockroachdb/cockroach/blob/f0bf32430c4960bfdad6d867e6df0e67079aeee1/pkg/ui/.claude/skills/redux-to-swr/SKILL.md) · 32206★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: redux-to-swr
description: Migrate React components from Redux + Saga to SWR hooks. Use when converting data fetching from Redux store (reducers, sagas, selectors, connect HOC) to SWR-based hooks in CockroachDB DB Console or cluster-ui.
---

# Redux + Saga to SWR Migration Guide

Migrate React components from Redux + redux-saga data fetching to SWR (stale-while-revalidate) hooks. The migration eliminates boilerplate (reducers, sagas, selectors, action creators, connected components) and replaces it with co-located data fetching hooks.

---

## Architecture

### Before (Redux + Saga)
```
Component (connected via mapStateToProps/mapDispatchToProps)
  -> dispatch(refresh()) action
  -> saga watches for action, calls API
  -> saga dispatches success/failure actions
  -> reducer updates store
  -> selector reads from store
  -> mapStateToProps feeds data to component
```

Files involved per feature:
- `store/<feature>/index.ts` — barrel export
- `store/<feature>/<feature>.reducer.ts` — Redux reducer
- `store/<feature>/<feature>.sagas.ts` — saga watchers/workers
- `store/<feature>/<feature>.sagas.spec.ts` — saga tests
- `store/<feature>/<feature>.selectors.ts` — selectors
- `sto
```

</details>
