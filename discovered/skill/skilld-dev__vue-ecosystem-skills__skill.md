---
name: skilld-dev__vue-ecosystem-skills__skill
source: https://github.com/skilld-dev/vue-ecosystem-skills/blob/4bf73fcada2497d6b6ef6142ff1d9d66cc1f27d5/skills/vuetify-skilld/SKILL.md
repo: skilld-dev/vue-ecosystem-skills
kind: skill
stars: 168
last_pushed: 2026-05-05T08:23:03Z
license: mit
score: 9
domains: [web-frontend, vue-js]
tags: [vuetify, ui-framework, migration-guide]
curated: 2026-06-15
curated_by: config-scout
---

# skilld-dev/vue-ecosystem-skills — skill

**Why it's worth keeping:** It uses 'Preferred vs Avoid' code blocks to teach pattern adherence and explicitly documents version-specific API shifts that prevent model hallucinations during migrations.

**Summary:** A high-density knowledge injection for Vuetify v4 that prioritizes breaking changes and architectural best practices.

**Source credibility:** High; the source repository shows active maintenance and significant community interest via stars.

**Recency:** Very current, specifically targeting the latest major version of the Vuetify ecosystem.

**Source:** [skilld-dev/vue-ecosystem-skills/skills/vuetify-skilld/SKILL.md](https://github.com/skilld-dev/vue-ecosystem-skills/blob/4bf73fcada2497d6b6ef6142ff1d9d66cc1f27d5/skills/vuetify-skilld/SKILL.md) · 168★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: vuetify-skilld
description: "Vue Material Component Framework. ALWAYS use when writing code importing \"vuetify\". Consult for debugging, best practices, or modifying vuetify."
metadata:
  version: 4.0.1
  generated_at: 2026-04-20
  references_synced_at: 2026-04-20
---

# vuetifyjs/vuetify `vuetify@4.0.1`
**Tags:** v1-stable: 1.5.24, v2-stable: 2.7.2, dev: 4.0.1

**References:** [Docs](./references/docs/_INDEX.md)
## API Changes

This section documents version-specific API changes — prioritize recent major/minor releases.

- BREAKING: `VRow` / `VCol` Grid — complete overhaul using CSS `gap` instead of negative margins. `dense` prop removed (use `density="compact"`), `align`/`justify` on `VRow` and `order`/`align-self` on `VCol` removed in favor of utility classes [source](./references/docs/src/pages/en/getting-started/upgrade-guide.md)

- BREAKING: MD3 Typography — variant names renamed for Material Design 3 compliance: `h1`-`h3` -> `display-*`, `h4`-`h6` -> `headline-*`, `subtitle-1`/`body-1` -> `body-large`, `button`/`subtitle-2` -> `label-large` [source](./references/docs/src/pages/en/getting-started/upgrade-guide.md)

- BREAKING: MD3 Elevation — elevation levels reduc
```

</details>
