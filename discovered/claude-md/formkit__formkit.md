---
name: formkit__formkit
source: https://github.com/formkit/formkit/blob/528d6e373555cca39c7ac24c1aa01af9ca18f9fd/CLAUDE.md
repo: formkit/formkit
kind: claude-md
stars: 4724
last_pushed: 2026-06-10T17:06:35Z
license: mit
score: 7
domains: [web-frontend, frameworks, vue-js]
tags: [architecture, command-reference, monorepo]
curated: 2026-06-16
curated_by: config-scout
---

# formkit/formkit — claude-md

**Why it's worth keeping:** The specific breakdown of the 'Node tree' and 'Schema expressions' gives an agent a precise structural mental model to prevent logic errors in complex state manipulations.

**Summary:** Provides a deep technical mental model of the system architecture alongside explicit operational commands.

**Source credibility:** Highly credible; FormKit is a well-maintained, popular Vue.js ecosystem library.

**Recency:** Current; uses modern toolchains like pnpm and Vitest.

**Source:** [formkit/formkit/CLAUDE.md](https://github.com/formkit/formkit/blob/528d6e373555cca39c7ac24c1aa01af9ca18f9fd/CLAUDE.md) · 4724★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# FormKit

Vue.js form building library. Monorepo with framework-agnostic core and Vue-specific integration.

## Architecture

**Node tree**: Every `<FormKit>` component owns a node (`packages/core/src/node.ts`). Three node types:
- `input`: single value (scalar, object, or array)
- `group`: children as object (keys = child names). `<FormKit type="form">` is a group.
- `list`: children as array

**Schema**: JSON-serializable data format for DOM/component structures. Rendered via `<FormKitSchema>`. Four node types:
- **Text**: plain strings
- **$el**: HTML elements (`{ $el: 'div', attrs: {}, children: [] }`)
- **$cmp**: Vue components (`{ $cmp: 'MyComponent', props: {} }`)
- **$formkit**: FormKit inputs (`{ $formkit: 'text', name: 'email' }`)—props flattened to top level

**Schema expressions**: `$`-prefixed references are reactive. `$: (value * 3)` for expressions not starting with reference. Supports arithmetic, comparison, logical operators. NOT JavaScript—compiled templating language with restricted execution.

**Schema features**:
- `if`/`then`/`else`: conditional rendering
- `for`: loops (like v-for)
- `bind`: dynamic attrs/props (like v-bind)
- `$slots`: access scoped slots
-
```

</details>
