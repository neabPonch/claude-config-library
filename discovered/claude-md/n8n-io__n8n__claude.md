---
name: n8n-io__n8n__claude
source: https://github.com/n8n-io/n8n/blob/f412820f522ab8cc3aa42097b618b046cb000288/packages/frontend/editor-ui/src/app/stores/workflowDocument/CLAUDE.md
repo: n8n-io/n8n
kind: claude-md
stars: 192561
last_pushed: 2026-06-15T06:34:36Z
license: other
score: 9
domains: [web-frontend, state-management, vuejs]
tags: [architecture, reactivity, composition-api, state-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# n8n-io/n8n — claude-md

**Why it's worth keeping:** The explicit instruction on emitting reactive proxies rather than raw objects solves a common Vue-specific pitfall, while the anti-pattern table prevents common architectural drift.

**Summary:** Defines a rigorous 'apply/public' method split for state mutation to ensure reactivity integrity and CRDT readiness. It provides strict rules for event notification and dependency injection.

**Source credibility:** Extremely high; n8n is a majorly starred, production-grade automation platform.

**Recency:** Current; uses modern Vue/composition API patterns and addresses complex state synchronization concerns.

**Source:** [n8n-io/n8n/packages/frontend/editor-ui/src/app/stores/workflowDocument/CLAUDE.md](https://github.com/n8n-io/n8n/blob/f412820f522ab8cc3aa42097b618b046cb000288/packages/frontend/editor-ui/src/app/stores/workflowDocument/CLAUDE.md) · 192561★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# workflowDocument store — Agent Guidelines

## Core pattern: apply/public method split

Every composable in this folder follows a two-layer pattern:

**Public methods** (exposed) — represent user intent. Handle normalization,
deduplication, and preparation. Call apply methods internally.

**Apply methods** (private) — the **only** functions that mutate refs. Each
apply method writes to the ref and fires an event hook. Never expose apply
methods from the composable.

```
Component → publicMethod() → normalize → applyXxx() → ref + event hook
```

This split exists to support CRDT in the future: local user actions,
remote CRDT sync, and undo/redo all converge on the same private apply
methods inside the composable.

## Event hooks

Every composable exposes change notifications via `createEventHook` from
`@vueuse/core`. Event payloads must extend `ChangeEvent` from `./types.ts`:

```typescript
import { createEventHook } from '@vueuse/core';
import type { ChangeEvent, ChangeAction } from './types';

type MyChangeEvent = ChangeEvent<{ /* domain-specific fields */ }>;
const onMyChange = createEventHook<MyChangeEvent>();
```

- Fire `void onMyChange.trigger(...)` inside every apply method
```

</details>
