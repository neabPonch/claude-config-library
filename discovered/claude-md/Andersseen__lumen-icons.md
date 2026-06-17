---
name: Andersseen__lumen-icons
source: https://github.com/Andersseen/lumen-icons/blob/f93c0fbe105c77eb1ad3cec4c5d17d0b207eef4f/CLAUDE.md
repo: Andersseen/lumen-icons
kind: claude-md
stars: 0
last_pushed: 2026-06-15T20:11:54Z
license: unknown
score: 9
domains: [web-frontend, angular]
tags: [component-library, design-system, typescript]
curated: 2026-06-16
curated_by: config-scout
---

# Andersseen/lumen-icons — claude-md

**Why it's worth keeping:** The inclusion of a 'Component template' and specific 'Rules' section prevents AI from generating non-compliant code; the detail on import paths/aliases is also excellent for preventing breakage.

**Summary:** This file provides rigorous technical documentation covering repository structure, command sets, and component-level implementation standards.

**Source credibility:** High-quality technical content despite zero stars, indicating a professional or highly organized personal project.

**Recency:** Extremely current, utilizing modern Angular 21 standards and Signals API.

**Source:** [Andersseen/lumen-icons/CLAUDE.md](https://github.com/Andersseen/lumen-icons/blob/f93c0fbe105c77eb1ad3cec4c5d17d0b207eef4f/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

---

## Project vision

An open-source Angular icon library inspired by projects like Lucide and Radix Icons but built specifically for Angular 21+. The library (`lumen-icons`) ships individual icon components with the `lmn-*` selector prefix. Icons are:

- **Tree-shakable by default** — each icon is its own entry point (`lumen-icons/icons/check`).
- **Accessible by default** — correct ARIA defaults, configurable `ariaLabel`.
- **Zero framework styling** — no Tailwind in the library; consumers control appearance.
- **Optionally animated** — animations via `angular-movement` (`MoveVariantsDirective`) + CSS `@keyframes` (opt-in per icon use).
- **Installable as a package** OR copy-pasteable as single files into any Angular project.

The companion `src/` application is the official demo + docs site, built with AnalogJS and styled with Tailwind CSS. The demo uses `@voltui/components` for its own UI chrome so development stays fast.

---

## Repository shape

```
lumen-icons/
├── packages/icons/          ← publishable library: lumen-icons
│   ├── src/
│   │   ├── index.ts
```

</details>
