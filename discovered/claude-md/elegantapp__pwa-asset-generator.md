---
name: elegantapp__pwa-asset-generator
source: https://github.com/elegantapp/pwa-asset-generator/blob/da32abea69510822a49f7c50df4388fb9fae0b82/CLAUDE.md
repo: elegantapp/pwa-asset-generator
kind: claude-md
stars: 3019
last_pushed: 2026-06-01T09:35:56Z
license: mit
score: 9
domains: [cli-tools, web-pwa, automation]
tags: [node.js, puppeteer, architecture-map, testing-guide]
curated: 2026-06-16
curated_by: config-scout
---

# elegantapp/pwa-asset-generator — claude-md

**Why it's worth keeping:** The 'Important design decisions' section provides critical context to prevent AI hallucinations regarding dependencies, while the detailed command breakdown includes advanced stress-testing instructions.

**Summary:** A comprehensive technical manual that maps the entire codebase, from high-level architecture to specific CLI commands and testing nuances.

**Source credibility:** Highly credible; a highly starred (3k+) well-maintained utility used in production workflows.

**Recency:** Very current; reflects modern TypeScript/Node.js patterns and up-to-date maintenance.

**Source:** [elegantapp/pwa-asset-generator/CLAUDE.md](https://github.com/elegantapp/pwa-asset-generator/blob/da32abea69510822a49f7c50df4388fb9fae0b82/CLAUDE.md) · 3019★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

pwa-asset-generator is a CLI tool and JavaScript module that automates PWA asset generation. It generates icon and splash screen images for Progressive Web Apps, automatically updating manifest.json and index.html files according to Web App Manifest specs and Apple Human Interface guidelines.

The tool uses Puppeteer to control a Chrome browser as a canvas, rendering images at various resolutions for different devices. It can scrape Apple's Human Interface guidelines website to get the latest device specifications or fall back to static data.

## Essential Commands

### Development workflow
```bash
npm install              # Install dependencies
npm run build            # Build TypeScript to dist/ (also copies JSON files)
npm run start            # Watch mode for TypeScript compilation
npm run lint             # Run ESLint
npm run lint:fix         # Fix ESLint issues
npm run prettier         # Check code formatting
npm run prettier:fix     # Auto-format code
npm run tsc              # Type check without emitting files
```

### Testing
```bash
npm
```

</details>
