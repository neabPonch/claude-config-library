---
name: wunki__amplify__skill
source: https://github.com/wunki/amplify/blob/2ebe24d92cb44cb557b55dbe753eb08a3959da12/skills/liveview-optimistic-ui/SKILL.md
repo: wunki/amplify
kind: skill
stars: 19
last_pushed: 2026-03-15T06:56:42Z
license: unknown
score: 9
domains: [web-frontend, elixir, phoenix-liveview]
tags: [optimistic-ui, ux-patterns, elixir, liveview]
curated: 2026-06-15
curated_by: config-scout
---

# wunki/amplify — skill

**Why it's worth keeping:** Provides specific, production-ready code patterns for composing JS commands, managing stream transitions with CSS timing delays, and handling async mutations via temporary IDs.

**Summary:** A highly specialized guide for implementing optimistic UI patterns in El\ixir Phoenix LiveView to ensure high perceived responsiveness.

**Source credibility:** High; the content demonstrates expert-level knowledge of Phoenix/LiveView edge cases like race conditions and stream synchronization.

**Recency:** Very recent (3 months ago) and includes modern LiveView features like stream_async.

**Source:** [wunki/amplify/skills/liveview-optimistic-ui/SKILL.md](https://github.com/wunki/amplify/blob/2ebe24d92cb44cb557b55dbe753eb08a3959da12/skills/liveview-optimistic-ui/SKILL.md) · 19★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: liveview-optimistic-ui
description: >
  Implements optimistic UI patterns in Elixir Phoenix LiveView: instant client
  feedback before server confirmation, loading states, rollback/revert on failure,
  race condition guards, stream insert/delete animations, undo windows, and
  accessibility for async interactions. Use when the user needs LiveView interactions
  to feel immediate, wants to add loading indicators or spinners, needs to handle
  double-submit or double-click, wants to animate stream inserts or deletes, needs
  undo/rollback for destructive actions, is dealing with stale data or flicker under
  latency, or needs aria-live announcements for optimistic state changes.
  Don't use for general LiveView form validation or changeset errors (use
  liveview-forms instead), non-LiveView frontend frameworks (React, Vue, Svelte),
  or server-side performance optimization unrelated to perceived UI responsiveness.
---

# LiveView Optimistic UI

Build LiveView interactions that feel instant while preserving server truth.

## Core Model

1. Keep data state on the server, visual feedback on the client.
2. Apply immediate client feedback first, then push the event.
3. Let serve
```

</details>
