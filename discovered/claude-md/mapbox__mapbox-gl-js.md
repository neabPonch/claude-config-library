---
name: mapbox__mapbox-gl-js
source: https://github.com/mapbox/mapbox-gl-js/blob/762299be2f93d9626fc1cf4900c94cec3a7d13de/CLAUDE.md
repo: mapbox/mapbox-gl-js
kind: claude-md
stars: 12305
last_pushed: 2026-06-15T07:46:52Z
license: other
score: 10
domains: [web-frontend, graphics]
tags: [high-performance, webgl, opinionated]
curated: 2026-06-15
curated_by: config-scout
---

# mapbox/mapbox-gl-js — claude-md

**Why it's worth keeping:** Includes specific 'banned' syntax patterns to prevent regressions and provides highly granular testing/command instructions essential for complex codebases.

**Summary:** Establishes strict technical guardrails and a deep architectural mental model for high-performance WebGL rendering.

**Source credibility:** High; Mapbox is an industry-standard, heavily maintained open-source project.

**Recency:** Current; the command patterns and workflow constraints are highly optimized for modern agentic coding tools.

**Source:** [mapbox/mapbox-gl-js/CLAUDE.md](https://github.com/mapbox/mapbox-gl-js/blob/762299be2f93d9626fc1cf4900c94cec3a7d13de/CLAUDE.md) · 12305★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

Mapbox GL JS is a JavaScript library for interactive, customizable vector maps on the web. It uses WebGL to render vector tiles that conform to the Mapbox Vector Tile Specification.

## Workflow
- Keep changes minimal and fully justified
- Always inspect a referenced file before explaining or fixing it
- Understand WHY code exists before changing it — GL JS has many browser quirks, performance hacks, and WebGL subtleties; check git blame when in doubt
- No abstractions or helpers until you see repetition, and only if cleaner than the duplication
- Always run `npm run tsc` and `npm run lint` when you're done making a series of code changes
- Run `npm run codegen` if you modify style properties or the style specification
- Run `npm run test-typings` after modifying public API types or the style specification
- Prefer running single tests, and avoid running the whole test suite, for performance
- Never add any dependencies unless explicitly requested

## Essential Commands

### Development

```bash
npm start
npm run build-esm-dev
npm run build-esm-prod
npm run build-prod # UMD build
npm run build-css
npm run codegen
```

### Testing

```bash
npm run t
```

</details>
