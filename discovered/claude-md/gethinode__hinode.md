---
name: gethinode__hinode
source: https://github.com/gethinode/hinode/blob/1b103c4ad37598974cacd05e392577d7983595b2/CLAUDE.md
repo: gethinode/hinode
kind: claude-md
stars: 187
last_pushed: 2026-06-11T14:08:46Z
license: mit
score: 9
domains: [web-frontend, static-site-generators]
tags: [architecture, hugo, templates, modular]
curated: 2026-06-14
curated_by: config-scout
---

# gethinode/hinode — claude-md

**Why it's worth keeping:** Uses clear 'ownership' definitions and provides structural code examples for complex, multi-layer templating architectures. This prevents the AI from incorrectly placing or modifying templates in a modular system.

**Summary:** Detailed architectural guide for a Hugo theme that explains module dependencies and component ownership. It explicitly defines the hierarchy between core and optional modules to prevent logic errors.

**Source credibility:** High: active development (0 months ago) and moderate GitHub stars suggest a real-world production tool.

**Recency:** Current; aligns with modern Hugo module and asset management practices.

**Source:** [gethinode/hinode/CLAUDE.md](https://github.com/gethinode/hinode/blob/1b103c4ad37598974cacd05e392577d7983595b2/CLAUDE.md) · 187★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Hinode is a Hugo theme for documentation and blog sites built on Bootstrap 5. It uses Hugo's module system to manage dependencies. The theme is designed for performance, security (with CSP headers), and SEO.

**Version 2 (templatev2 branch)** is a minimal core theme. Optional extensions like mod-blocks add features like pre-built Bookshop components for page building.

## Common Development Commands

### Development Server

```bash
npm start                    # Start Hugo server with module vendoring
npm run start:example        # Start server using exampleSite
npm run start:prod          # Start server in production mode
npm run start:example:prod  # Start exampleSite in production mode
```

### Building

```bash
npm run build               # Build site with minification
npm run build:example       # Build exampleSite
npm run build:debug         # Build with debug output
npm run build:headers       # Generate Netlify/server headers
```

### Linting & Testing

```bash
npm test                    # Run all linters
npm run lint                # Run all li
```

</details>
