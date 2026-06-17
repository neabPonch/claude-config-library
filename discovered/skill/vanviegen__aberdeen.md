---
name: vanviegen__aberdeen
source: https://github.com/vanviegen/aberdeen/blob/fbe927ebbe39649305a6c12d5dc97e9a25e1bbb0/SKILL.md
repo: vanviegen/aberdeen
kind: skill
stars: 106
last_pushed: 2026-06-15T07:51:50Z
license: isc
score: 8
domains: [web-frontend, typescript]
tags: [reactivity, performance-optimization, ui-library]
curated: 2026-06-15
curated_by: config-scout
---

# vanviegen/aberdeen — skill

**Why it's worth keeping:** It includes actionable 'anti-patterns' (e.g., avoiding manual array iteration and data concatenation) that prevent common logic errors specific to proxy-based state management.

**Summary:** Provides specialized developer guidelines for the Aberdeen reactive UI library, focusing on maintaining high performance through fine-grained reactivity rules.

**Source credibility:** The library is niche with 106 stars, but the documentation depth suggests a well-thought-out architectural pattern.

**Recency:** Current; follows modern TypeScript patterns and provides high-signal instructions for AI agents.

**Source:** [vanviegen/aberdeen/SKILL.md](https://github.com/vanviegen/aberdeen/blob/fbe927ebbe39649305a6c12d5dc97e9a25e1bbb0/SKILL.md) · 106★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: aberdeen
description: Expert guidance for building reactive UIs with the Aberdeen library. Covers element creation, reactive proxy state, efficient list rendering, CSS shortcuts, UI components, routing, transitions, and optimistic updates.
---

Aberdeen is a reactive UI library using fine-grained reactivity via JavaScript Proxies. No virtual DOM, no build step required.

# Guidance for AI Assistants

1. **Never concatenate user data** - Use `A('input value=', data)` not `A('input value=${data}')`
2. **Pass observables directly** - Use `text=', ref(obj, 'key')` to avoid parent scope subscriptions
3. **Use `onEach` for lists** - Never iterate proxy arrays with `for`/`map` in render functions
4. **Class instances are great** - Better than plain objects for typed, structured state
5. **CSS shortcuts** - Use $3, $4 for spacing (1rem, 2rem), $primary for colors (assuming setVarSpacingCssVars is used and cssVars colors are defined)
6. **Minimal scopes** - Smaller reactive scopes = fewer DOM updates
7. **Function components** - Create reusable UI components as regular functions starting with 'draw' (like drawMainMenu(settings) or drawProfilePage(user))
8. **Prefix proxied objects
```

</details>
