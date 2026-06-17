---
name: GetStream__stream-chat-react__skill
source: https://github.com/GetStream/stream-chat-react/blob/a7e9006d69a9e3b251ab6386ef62182712d87f65/.cursor/skills/accessibility/SKILL.md
repo: GetStream/stream-chat-react
kind: skill
stars: 838
last_pushed: 2026-06-12T15:46:38Z
license: other
score: 9
domains: [web-frontend, accessibility]
tags: [a11y, react, i18n, testing]
curated: 2026-06-15
curated_by: config-scout
---

# GetStream/stream-chat-react — skill

**Why it's worth keeping:** Includes highly actionable 'where to put what' mappings and an execution checklist that prevents the agent from guessing file locations or breaking i18n patterns.

**Summary:** A rigorous specification for maintaining WCAG compliance and semantic integrity within a React component library.

**Source credibility:** High; derived from a mature, widely-used enterprise React SDK (Stream Chat).

**Recency:** Very current, adhering to modern web accessibility and i18n standards.

**Source:** [GetStream/stream-chat-react/.cursor/skills/accessibility/SKILL.md](https://github.com/GetStream/stream-chat-react/blob/a7e9006d69a9e3b251ab6386ef62182712d87f65/.cursor/skills/accessibility/SKILL.md) · 838★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: accessibility
description: Maintain WCAG-focused accessibility in stream-chat-react. Use when changing interactive components, dialogs, menus, forms, media controls, notifications, focus behavior, keyboard flows, aria attributes, or screen-reader announcements.
---

# Accessibility Maintenance (stream-chat-react)

Use this skill whenever code changes can affect keyboard users, screen readers, focus behavior, motion preferences, or semantic HTML/ARIA.

## Non-negotiable rules

1. Prefer native semantics first (`button`, `input`, `label`, `img`, etc.). Use ARIA roles only when native semantics cannot represent the widget.
2. Do not add hardcoded English accessibility labels. Use i18n keys (`t('aria/...')`) for user-facing `aria-label`/`aria-description`/announcement strings.
3. Keep one focusable interactive target per action. Avoid duplicate focus stops and nested-interactive patterns.
4. If a control is keyboard-activatable, support Enter/Space behavior and visible focus.
5. Decorative visuals stay hidden from AT (`aria-hidden`, `focusable="false"` for SVG icons).
6. Keep changes additive and backward-compatible for SDK consumers.

## Where to put what

- **Cross-cutting
```

</details>
