---
name: yysun__apprun
source: https://github.com/yysun/apprun/blob/b56dae0cbcabc63c5a364da363bc2e8c80160020/SKILL.md
repo: yysun/apprun
kind: skill
stars: 1175
last_pushed: 2026-04-03T17:54:15Z
license: mit
score: 8
domains: [web-frontend, typescript]
tags: [apprun, mvu, vite, boilerplate]
curated: 2026-06-14
curated_by: config-scout
---

# yysun/apprun — skill

**Why it's worth keeping:** Includes critical 'tsconfig' mappings required for custom JSX factories and provides a standardized API client pattern that is highly transferable.

**Summary:** Provides a comprehensive architectural blueprint for AppRun applications, including specific Vite and TypeScript configurations.

**Source credibility:** High; based on an active, well-regarded open-source library (apprun).

**Recency:** Current; includes modern setup instructions like Tailwind CSS v4 integration.

**Source:** [yysun/apprun/SKILL.md](https://github.com/yysun/apprun/blob/b56dae0cbcabc63c5a364da363bc2e8c80160020/SKILL.md) · 1175★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: apprun-skills
description: End-to-end guidance for AppRun apps in TypeScript using MVU including component patterns, event handling, state management (including async generators), routing/navigation with params and guards, and testing with vitest. Use when designing or reviewing AppRun components, wiring routes, managing state flows, or writing AppRun tests.
---

# AppRun Skills

## Overview

- Build AppRun apps with MVU (Model-View-Update) in TypeScript.
- Prefer pure update functions for testability.
- Use `mounted()` for components embedded in JSX.
- Use `state = async` only for top-level routed pages that must load async data.

## Project Setup

### Recommended Project Structure

```
web/                        # Frontend application root
├── index.html              # Entry HTML file
├── package.json            # Dependencies and scripts
├── vite.config.js          # Vite configuration
├── src/
│   ├── main.tsx            # Application entry point (routes registration)
│   ├── api.ts              # REST API client (optional)
│   ├── styles.css          # Application styles
│   ├── tsconfig.json       # TypeScript configuration
│   ├── components/         # Reusable UI
```

</details>
