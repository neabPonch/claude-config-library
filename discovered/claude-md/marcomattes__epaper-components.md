---
name: marcomattes__epaper-components
source: https://github.com/marcomattes/epaper-components/blob/e4116a03285dea32a07499a6107ec72c047aa8fe/claude.md
repo: marcomattes/epaper-components
kind: claude-md
stars: 22
last_pushed: 2026-04-26T06:43:38Z
license: mit
score: 9
domains: [web-frontend, design-systems]
tags: [css, web-components, e-ink, accessibility, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# marcomattes/epaper-components — claude-md

**Why it's worth keeping:** The `:where()` specificity strategy and dual-target selector pattern (`.class` + `element`) are elite techniques for creating scalable component libraries. The execution plan enforces a strict architectural hierarchy that prevents AI hallucinations during complex builds.

**Summary:** Provides a sophisticated blueprint for building a high-constraint, zero-JS design system optimized for E-Ink displays. It integrates CSS variables, theme switching, and Web Component progressive enhancement.

**Source credibility:** High-quality technical instructions despite the small repository size, reflecting senior design-system expertise.

**Recency:** Very current; leverages modern CSS features like `:where()` and attribute-based theming patterns.

**Source:** [marcomattes/epaper-components/claude.md](https://github.com/marcomattes/epaper-components/blob/e4116a03285dea32a07499a6107ec72c047aa8fe/claude.md) · 22★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# E‑Paper Components Library — Claude Brief

Use this repo to generate a no-JS component library and demo pages optimized for E‑Ink readers (Kindle/Tolino class). Follow the steps and constraints exactly.

## Persona & Goal

- Act as a senior design-system engineer for E‑Paper Componentss.
- Deliver working HTML/CSS only: tokens, base, components, demos, README. No JavaScript anywhere.

## Execution Plan (must follow in order)

1. Propose the final architecture (tokens, layers, components, pages). Keep it minimal.
2. Define tokens in `epaper-components.tokens.css`.
3. Define reset/base in `epaper-components.base.css`.
4. Implement components in `epaper-components.components.css`.
5. Generate demo pages:
   - `demo/index.html` (overview + navigation)
   - `demo/typography.html`
   - `demo/layout.html`
   - `demo/components.html` (Cards, Buttons, Inputs, Select, Checkbox/Radio, Table, Picture)
   - `demo/forms.html` (validation states, help text, disabled, required, error summary pattern)
   - `demo/dialog.html` (native `<dialog>` patterns and fallback notes)
   - `demo/tables.html` (table patterns + responsive strategy without JS)
     Each page must import the CSS files and show al
```

</details>
