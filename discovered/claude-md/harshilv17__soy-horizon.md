---
name: harshilv17__soy-horizon
source: https://github.com/harshilv17/soy-horizon/blob/a35bfec5a1118ab43bb4f5824891379c14f67889/CLAUDE.md
repo: harshilv17/soy-horizon
kind: claude-md
stars: 1
last_pushed: 2026-06-14T07:08:34Z
license: other
score: 9
domains: [web-frontend, e-commerce]
tags: [shopify, liquid, css-bem, architecture-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# harshilv17/soy-horizon — claude-md

**Why it's worth keeping:** The instruction to modify JS schema sources instead of liquid blocks prevents the AI from making common manual configuration errors. The detailed component lifecycle and CSS specificity rules provide high-quality guardrails for an LLM.

**Summary:** Provides highly specific architectural constraints and a critical 'source-of-truth' workflow for generating Shopify schema files. It defines strict coding standards for JavaScript (Web Components), CSS (BEM/Specificity), and Liquid documentation.

**Source credibility:** High technical depth suggests a professional custom Shopify development environment despite low star count.

**Recency:** Current; uses modern web standards like logical properties and AbortController.

**Source:** [harshilv17/soy-horizon/CLAUDE.md](https://github.com/harshilv17/soy-horizon/blob/a35bfec5a1118ab43bb4f5824891379c14f67889/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

```bash
# Start local dev server (connects to a Shopify store)
shopify theme serve

# Lint and validate Liquid templates
shopify theme check

# After editing schema source files (schemas/ folder), regenerate .liquid files
npm run build:schemas
```

There is no build step for CSS or JavaScript — this is a server-rendered Shopify Liquid theme. All assets are plain CSS and vanilla JS served directly.

## Architecture Overview

This is **Horizon**, Shopify's flagship theme, customised as "Shades of You". It follows a strict web-native, server-rendered philosophy: no bundlers, no external JS dependencies, no polyfills.

### Directory Structure

| Directory | Purpose |
|-----------|---------|
| `sections/` | Page sections (`.liquid` for reusable, `.json` for section groups) |
| `blocks/` | Sub-components used within sections, filenames prefixed with `_` |
| `snippets/` | Reusable partials included via `{% render 'name' %}` |
| `assets/` | Plain CSS and JS files (no bundling) |
| `templates/` | JSON-based page templates (product, collection, cart, e
```

</details>
