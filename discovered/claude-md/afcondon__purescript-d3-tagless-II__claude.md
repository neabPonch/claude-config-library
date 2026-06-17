---
name: afcondon__purescript-d3-tagless-II__claude
source: https://github.com/afcondon/purescript-d3-tagless-II/blob/b3dac018d0a343b9db66fbaac87123fe9867af22/notes/CLAUDE.md
repo: afcondon/purescript-d3-tagless-II
kind: claude-md
stars: 39
last_pushed: 2026-04-04T16:52:37Z
license: mit
score: 9
domains: [web-frontend, functional-programming, data-visualization]
tags: [purescript, d3, monorepo, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# afcondon/purescript-d3-tagless-II — claude-md

**Why it's worth keeping:** Includes high-level design rationale (e.g., state isolation decisions) that prevents AI from proposing non-idiomatic changes, and provides specific toolchain versions to ensure build accuracy.

**Summary:** Provides a comprehensive structural map of a complex PureScript monorepo along with detailed architectural patterns.

**Source credibility:** A specialized niche library with recent maintenance activity.

**Recency:** Current; reflects modern Spago/PureScript environments.

**Source:** [afcondon/purescript-d3-tagless-II/notes/CLAUDE.md](https://github.com/afcondon/purescript-d3-tagless-II/blob/b3dac018d0a343b9db66fbaac87123fe9867af22/notes/CLAUDE.md) · 39★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a PureScript library implementing a Finally Tagless embedded DSL for building interactive data visualizations. The library wraps D3.js functionality in a purely functional, composable API with strong type safety. The project targets PureScript 0.15.

## Repository Structure

This is a **Spago monorepo** with four packages:

```
├── psd3-selection/       # Core D3 selection/attribute library (publishable)
│   ├── spago.yaml        # Package config only
│   └── src/PSD3/         # Selection, attributes, layouts, interpreters
├── psd3-simulation/      # Force simulation library (publishable)
│   ├── spago.yaml        # Depends on psd3-selection
│   └── src/PSD3/         # ForceEngine, Config
├── psd3-tidal/           # TidalCycles mini-notation parser (publishable)
│   ├── spago.yaml        # Standalone package
│   └── src/Tidal/        # AST, Parser, Pretty-printer
├── demo-website/         # Documentation and examples website
│   ├── spago.yaml        # Depends on all libraries
│   ├── src/              # Halogen components, visualizations
```

</details>
