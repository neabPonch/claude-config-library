---
name: sanity-io__next-sanity__skill
source: https://github.com/sanity-io/next-sanity/blob/b2be24e8da81588aa540d9d7f79bc5464ef9fdcf/.agents/skills/tsdown/SKILL.md
repo: sanity-io/next-sanity
kind: skill
stars: 947
last_pushed: 2026-06-14T03:35:02Z
license: mit
score: 9
domains: [cli-tools, web-frontend]
tags: [bundler, typescript, build-tool]
curated: 2026-06-15
curated_by: config-scout
---

# sanity-io/next-sanity — skill

**Why it's worth keeping:** The tabular format maps specific config keys to practical code snippets, which is ideal for zero-hallucination tool orchestration. It provides explicit patterns for complex tasks like custom dependency bundling logic.

**Summary:** A highly structured technical reference for the tsdown bundler, covering configuration, dependency management, and output options.

**Source credibility:** High; follows professional documentation standards found in top-tier developer tools.

**Recency:** Current; leverages modern build technologies such as Rolldown and Oxc.

**Source:** [sanity-io/next-sanity/.agents/skills/tsdown/SKILL.md](https://github.com/sanity-io/next-sanity/blob/b2be24e8da81588aa540d9d7f79bc5464ef9fdcf/.agents/skills/tsdown/SKILL.md) · 947★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: tsdown
description: Bundle TypeScript and JavaScript libraries with blazing-fast speed powered by Rolldown. Use when building libraries, generating type declarations, bundling for multiple formats, or migrating from tsup.
---

# tsdown - The Elegant Library Bundler

Blazing-fast bundler for TypeScript/JavaScript libraries powered by Rolldown and Oxc.

## When to Use

- Building TypeScript/JavaScript libraries for npm
- Generating TypeScript declaration files (.d.ts)
- Bundling for multiple formats (ESM, CJS, IIFE, UMD)
- Optimizing bundles with tree shaking and minification
- Migrating from tsup with minimal changes
- Building React, Vue, Solid, or Svelte component libraries

## Quick Start

```bash
# Install
pnpm add -D tsdown

# Basic usage
npx tsdown

# With config file
npx tsdown --config tsdown.config.ts

# Watch mode
npx tsdown --watch

# Migrate from tsup
npx tsdown-migrate
```

## Basic Configuration

```ts
import {defineConfig} from 'tsdown'

export default defineConfig({
  entry: ['./src/index.ts'],
  format: ['esm', 'cjs'],
  dts: true,
  clean: true,
})
```

## Core References

| Topic              | Description                                       | Referenc
```

</details>
