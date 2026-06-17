---
name: duvall-here-and-now__here-and-now-spa
source: https://github.com/duvall-here-and-now/here-and-now-spa/blob/06854439248551d30e7584cc9186ab5b5f667893/CLAUDE.md
repo: duvall-here-and-now/here-and-now-spa
kind: claude-md
stars: 0
last_pushed: 2026-06-13T20:07:37Z
license: apache-2.0
score: 9
domains: [web-frontend, angular]
tags: [angular, auth0, azure, typescript, spa]
curated: 2026-06-17
curated_by: config-scout
---

# duvall-here-and-now/here-and-now-spa — claude-md

**Why it's worth keeping:** The architecture section explains a specific complex environment-to-build transformation (env to environment.ts), while coding standards provide actionable guidance on OnPush detection and ARIA accessibility handling.

**Summary:** A highly detailed technical guide for an Angular 18 SPA featuring Auth0 and Azure deployment. It provides clear architectural patterns, environment configuration workflows, and strict Git protocols.

**Source credibility:** Single-user repo with recent activity; appears to be a legitimate, professional-grade project setup.

**Recency:** Very current, utilizing Angular 18 and modern TypeScript patterns.

**Source:** [duvall-here-and-now/here-and-now-spa/CLAUDE.md](https://github.com/duvall-here-and-now/here-and-now-spa/blob/06854439248551d30e7584cc9186ab5b5f667893/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an Angular 18 Single-Page Application (SPA) demonstrating user authentication with Auth0. The application is deployed to Azure Static Web Apps and communicates with a backend API for protected resources.

## Essential Commands

### Development
```bash
npm run start          # Run dev server with environment setup (http://0.0.0.0:4040)
npm run env            # Generate environment.ts from .env file
ng serve               # Run dev server without env setup
npm run watch          # Build in watch mode
```

### Build
```bash
npm run build          # Production build (runs env setup first)
ng build               # Build without env setup
```

### Testing
```bash
ng test                # Run Karma tests in Chrome
ng test --no-watch --code-coverage  # Single test run with coverage
```

## Git Workflow

**IMPORTANT**: This is a collaborative environment. Always maintain user control over git operations:

- **NEVER push code to any branch without explicit user approval**
- **NEVER create new branches without asking first**
- **NEVER create pull re
```

</details>
