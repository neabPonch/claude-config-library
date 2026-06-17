---
name: onmax__nuxt-skills__skill
source: https://github.com/onmax/nuxt-skills/blob/311074589914796ad39356bf42ab68f920ebee04/skills/tsdown/SKILL.md
repo: onmax/nuxt-skills
kind: skill
stars: 683
last_pushed: 2026-06-01T07:41:14Z
license: unknown
score: 9
domains: [cli-tools, web-frontend, build-systems]
tags: [bundler, typescript, context-management, dev-tools]
curated: 2026-06-15
curated_by: config-scout
---

# onmax/nuxt-skills — skill

**Why it's worth keeping:** Implements advanced context management by explicitly instructing the agent NOT to load all files at once and mapping specific tasks to targeted reference docs.

**Summary:** Acts as a hierarchical router for 'tsdown' documentation, providing task-specific entry points rather than overwhelming the context window.

**Source credibility:** High; 683 stars on GitHub indicates a significant, community-validated utility within the Nuxt ecosystem.

**Recency:** 

**Source:** [onmax/nuxt-skills/skills/tsdown/SKILL.md](https://github.com/onmax/nuxt-skills/blob/311074589914796ad39356bf42ab68f920ebee04/skills/tsdown/SKILL.md) · 683★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: tsdown
description: Use when bundling TypeScript libraries - provides tsdown configuration, dual ESM/CJS output, .d.ts generation, package validation, and plugin authoring
license: MIT
---

# tsdown

Rolldown + Oxc powered TypeScript bundler. Drop-in tsup replacement.

## When to Use

- Building TypeScript libraries
- Generating .d.ts declarations
- Publishing npm packages
- Dual ESM/CJS output
- Vue/React component libraries

## Quick Start

```bash
npm i -D tsdown typescript
```

```ts
// tsdown.config.ts
import { defineConfig } from 'tsdown'

export default defineConfig({
  entry: 'src/index.ts',
  format: 'esm',
  dts: true,
  exports: true,
})
```

```bash
tsdown           # Build
tsdown --watch   # Watch mode
```

## Reference Files

| Task                                          | File                                  |
| --------------------------------------------- | ------------------------------------- |
| Config file, CLI, entry points                | [config.md](references/config.md)     |
| Format, target, dts, exports, validation      | [output.md](references/output.md)     |
| Shims, unbundle, watch, frameworks, WASM      | [features.md](references/featu
```

</details>
