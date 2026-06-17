---
name: oneo-me__breach-tab
source: https://github.com/oneo-me/breach-tab/blob/9c449e3aa78ed0f9231c0cfd215f55e1f3a01594/CLAUDE.MD
repo: oneo-me/breach-tab
kind: claude-md
stars: 0
last_pushed: 2025-12-24T11:29:40Z
license: unknown
score: 8
domains: [web-extension, frontend]
tags: [wxt, svelte5, tailwind-v4, browser-extension]
curated: 2026-06-16
curated_by: config-scout
---

# oneo-me/breach-tab — claude-md

**Why it's worth keeping:** The 'Common Tasks' section provides actionable instructions for extending the project, while the coding standards clearly define modern stack usage (Svelte 5/Tailwind v4).

**Summary:** A comprehensive technical specification for a WXT and Svelte 5 based browser extension.

**Source credibility:** Zero stars on GitHub, but the technical depth suggests a high-quality personal project.

**Recency:** 

**Source:** [oneo-me/breach-tab/CLAUDE.MD](https://github.com/oneo-me/breach-tab/blob/9c449e3aa78ed0f9231c0cfd215f55e1f3a01594/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project Overview

This is a browser extension built with WXT (Web Extension Toolkit) and Svelte 5. The extension provides two main features:
1. **New Tab Redirect**: Automatically redirects new tabs to a user-configured URL
2. **Popup Window Opener**: Opens the current tab in a new popup window with responsive device size presets

## Tech Stack

- **Framework**: WXT (Web Extension Toolkit)
- **UI Library**: Svelte 5
- **Language**: TypeScript
- **Build Tool**: Vite (via WXT)
- **Package Manager**: Bun
- **Styling**: Tailwind CSS v4
- **Linter/Formatter**: Biome.js

## Project Structure

```
breach-tab/
├── src/
│   ├── entrypoints/          # Extension entry points
│   │   ├── newtab/           # New tab redirect entry point
│   │   │   ├── index.html    # Newtab HTML template
│   │   │   └── main.ts       # Redirect logic
│   │   └── popup/            # Extension popup UI
│   │       ├── App.svelte    # Main popup component (device presets)
│   │       ├── main.ts       # Popup entry point
│   │       ├── index.html    # Popup HTML template
│   │       └── app.css       # Popup styles (with Tailwind CSS)
│   ├── lib/                  # Reusable Svelte components
│   │   └── Icon
```

</details>
