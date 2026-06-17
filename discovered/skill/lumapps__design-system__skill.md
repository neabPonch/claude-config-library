---
name: lumapps__design-system__skill
source: https://github.com/lumapps/design-system/blob/53633395a7c68adea45bd5b9640c6418fcb9d11f/.claude/skills/vue-docs/SKILL.md
repo: lumapps/design-system
kind: skill
stars: 25
last_pushed: 2026-06-15T16:51:10Z
license: mit
score: 8
domains: [web-frontend, documentation, migration]
tags: [vue, react, design-system, documentation]
curated: 2026-06-15
curated_by: config-scout
---

# lumapps/design-system — skill

**Why it's worth keeping:** It provides explicit cross-framework mapping rules (props, events, and state conversion) and a rigorous multi-step verification workflow.

**Summary:** A highly detailed migration skill that automates the process of adding Vue documentation alongside existing React docs.

**Source credibility:** High; derived from an active, professional design system repository.

**Recency:** Current; utilizes modern Vue 3 (script setup) and React patterns.

**Source:** [lumapps/design-system/.claude/skills/vue-docs/SKILL.md](https://github.com/lumapps/design-system/blob/53633395a7c68adea45bd5b9640c6418fcb9d11f/.claude/skills/vue-docs/SKILL.md) · 25★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: vue-docs
description: >
    Add or update Vue documentation for a component: Vue demo files (.vue SFCs), PropTable integration
    (props/events/slots), and MDX page updates. Use when a component in @lumx/vue needs Vue demos
    or prop table documentation added alongside existing React documentation.
---

# Vue Component Documentation

Add Vue documentation for a component on the site-demo documentation site: demo files, prop table integration, and MDX page wiring.

For general documentation site conventions (page structure, frontmatter, DemoBlock, PropTable, file layout), see `packages/site-demo/README.md`.

## Prerequisites

1. The component must exist in `@lumx/vue` (check `packages/lumx-vue/src/components/`)
2. An MDX page should exist at `packages/site-demo/content/product/components/<component>/index.mdx`
3. React demos should exist in `packages/site-demo/content/product/components/<component>/react/`

## Steps

### Step 1: Gather Context

1. **Read the React demos** in `content/product/components/<component>/react/`
2. **Read the MDX page** at `content/product/components/<component>/index.mdx`
3. **Check available Vue components** by reading `packages/lumx-vue/src
```

</details>
