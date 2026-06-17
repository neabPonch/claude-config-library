---
name: srod__node-minify
source: https://github.com/srod/node-minify/blob/566a7660881820fa86422ee2b9d38cf204a2d436/SKILL.md
repo: srod/node-minify
kind: skill
stars: 519
last_pushed: 2026-06-11T22:48:50Z
license: mit
score: 9
domains: [web-frontend, cli-tools, devops]
tags: [minification, node.js, asset-optimization, build-tools]
curated: 2026-06-15
curated_by: config-scout
---

# srod/node-minify — skill

**Why it's worth keeping:** The 'Compressor Selection' table provides essential decision logic for an agent, while the 'Common Patterns' section offers concrete code templates for complex tasks like globbing and image conversion.

**Summary:** A highly structured skill file for automating asset minification and optimization using the node-minify ecosystem.

**Source credibility:** High; well-maintained repository with significant community validation (519 stars).

**Recency:** Very current; includes modern tool recommendations like esbuild and lightningcss.

**Source:** [srod/node-minify/SKILL.md](https://github.com/srod/node-minify/blob/566a7660881820fa86422ee2b9d38cf204a2d436/SKILL.md) · 519★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: node-minify
description: |
  Compress JavaScript, CSS, HTML, JSON, and image files using node-minify library.
  Use when: minifying/compressing assets, bundling JS/CSS files, optimizing images (WebP/AVIF),
  concatenating files, or when user mentions "node-minify", "@node-minify", "minification".
  Triggers: "minify", "compress JS/CSS", "bundle", "optimize images", "reduce file size".
---

# node-minify

Lightweight Node.js minification library supporting JS, CSS, HTML, JSON, and images.

## Installation

```bash
# Core + compressor(s)
npm install @node-minify/core @node-minify/terser
```

## Quick Start

```ts
import { minify } from "@node-minify/core";
import { terser } from "@node-minify/terser";

// File-based
await minify({
  compressor: terser,
  input: "src/app.js",
  output: "dist/app.min.js",
});

// In-memory
const result = await minify({
  compressor: terser,
  content: "const x = 1; const y = 2;",
});
```

## Compressor Selection

| Type | Recommended | Alternatives |
|------|-------------|--------------|
| **JS** | `terser` (modern, fast) | `esbuild` (fastest), `swc`, `oxc`, `uglify-js`, `google-closure-compiler` (advanced optimizations, requires Java) |
| **
```

</details>
