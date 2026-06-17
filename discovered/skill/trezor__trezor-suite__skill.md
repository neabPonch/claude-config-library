---
name: trezor__trezor-suite__skill
source: https://github.com/trezor/trezor-suite/blob/c7924a79f7e31d480ca3d180de5bc28d1c57302a/skills/components/SKILL.md
repo: trezor/trezor-suite
kind: skill
stars: 1013
last_pushed: 2026-06-16T04:31:17Z
license: other
score: 8
domains: [web-frontend, react]
tags: [component-structure, state-management, performance]
curated: 2026-06-16
curated_by: config-scout
---

# trezor/trezor-suite — skill

**Why it's worth keeping:** Provides specific ordering rules for hooks/state to reduce cognitive load and mandates granular prop passing to optimize re-renders.

**Summary:** Defines a strict organizational hierarchy for React component files and internal logic structure.

**Source credibility:** High; Trezor is a highly-starred, professional security-focused repository.

**Recency:** Current; follows modern React best practices regarding component organization and performance.

**Source:** [trezor/trezor-suite/skills/components/SKILL.md](https://github.com/trezor/trezor-suite/blob/c7924a79f7e31d480ca3d180de5bc28d1c57302a/skills/components/SKILL.md) · 1013★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: components
description: React component file structure and patterns for Trezor Suite. Use when creating or reviewing React components, including prop passing and component organization.
---

# Components

## 🟠 File structure

1. ↕️ Imports
2. 🎨 Styles
3. 📜 Component constants
4. 🛠 Component helpers
5. 🆎 Component types
6. 🎭 Component prop type
7. 🍱 Component

## 🟠 Component structure

The following structure is just a recommendation, in fact it's not even always possible to keep the same order inside a component. However, trying to be consistent really helps in the long run, especially when it comes to navigating larger components. It is also useful to group things within each category, e.g. the refs might not have empty lines between each other but if there is only one `useDispatch` better surround it with them.

1. Redux selectors _(aka global state)_
2. `useState` _(aka local state)_
3. Non-effect hooks: `useRef`, `useForm`, `useDispatch`, etc
    1. This one is tricky. Consistency among the non-effect hook order is perhaps too redundant, although I would always put `useForm` first, for example. Try to place them in the order of subjective importance.
4. Effects
5. Fun
```

</details>
