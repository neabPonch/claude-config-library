---
name: PrestaShop__PrestaShop__skill
source: https://github.com/PrestaShop/PrestaShop/blob/c4af2a06adb1b7b4d2b85340a7e16def829dec35/.ai/Component/Javascript/skills/create-ts-entry-point/SKILL.md
repo: PrestaShop/PrestaShop
kind: skill
stars: 9107
last_pushed: 2026-06-15T15:16:35Z
license: other
score: 8
domains: [web-frontend, build-systems, e-commerce]
tags: [typescript, webpack, admin-panel, boilerplate]
curated: 2026-06-16
curated_by: config-scout
---

# PrestaShop/PrestaShop — skill

**Why it's worth keeping:** It treats development as a multi-step ritual that includes mandatory build-system updates (Webpack) and provides clear 'rules' to prevent common integration errors.

**Summary:** Automates the creation of TypeScript entry points for PrestaShop admin pages, including directory structuring and Webpack registration.

**Source credibility:** High; sourced from the official PrestaShop repository which is highly active and widely used.

**Recency:** Current; utilizes modern TypeScript/Webpack patterns suitable for modern agentic workflows.

**Source:** [PrestaShop/PrestaShop/.ai/Component/Javascript/skills/create-ts-entry-point/SKILL.md](https://github.com/PrestaShop/PrestaShop/blob/c4af2a06adb1b7b4d2b85340a7e16def829dec35/.ai/Component/Javascript/skills/create-ts-entry-point/SKILL.md) · 9107★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: create-ts-entry-point
description: >
  Create the TypeScript entry point files for a new admin page. Covers the directory
  structure, listing and form entry points, and webpack registration. References
  init-js-components and init-grid-extensions for component/extension details.
  Trigger: "create JS entry point for {Domain}".
needs: []
produces: "admin-dev/themes/new-theme/js/pages/{domain}/ — TypeScript entry points + webpack entry"
---

# create-ts-entry-point

Read `@.ai/Component/Javascript/CONTEXT.md` for the page structure and webpack config.

## 1. Directory structure

Create `admin-dev/themes/new-theme/js/pages/{domain}/`:

```
{domain}/
├── index.ts              # Listing page entry point
├── form.ts               # Form page entry point (simple)
│   OR form/index.ts      # Form page entry point (complex, with sub-files)
└── {domain}-map.ts       # DOM selector mappings (optional, for pages with many selectors)
```

For simple pages, `index.ts` and `form.ts` are enough. Only create subdirectories and manager classes for genuinely complex pages.

## 2. Listing entry point (`index.ts`)

Initializes the Grid instance and adds extensions. See `init-grid-extensions
```

</details>
