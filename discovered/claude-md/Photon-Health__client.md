---
name: Photon-Health__client
source: https://github.com/Photon-Health/client/blob/6f0b9d3435c0d9a94120c688562a227ef265a841/CLAUDE.md
repo: Photon-Health/client
kind: claude-md
stars: 3
last_pushed: 2026-06-13T00:31:46Z
license: unknown
score: 9
domains: [web-frontend, monorepo]
tags: [nx, react, solidjs, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# Photon-Health/client — claude-md

**Why it's worth keeping:** It defines strict 'never import' rules to prevent cross-framework JSX errors between Solid.js and React, and provides context for custom manual testing tools like bookmarklets.

**Summary:** A highly detailed guide for a complex monorepo containing specific operational commands and critical architectural boundaries.

**Source credibility:** Professional-grade healthcare project with active maintenance.

**Recency:** 

**Source:** [Photon-Health/client/CLAUDE.md](https://github.com/Photon-Health/client/blob/6f0b9d3435c0d9a94120c688562a227ef265a841/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Photon Health client monorepo — a healthcare platform with a clinical provider app and a patient-facing app, plus shared packages (components, SDK, elements).

## Common Commands

### Development

```bash
npm i                         # Install all dependencies
npm nx run app:pullenv        # Get env vars for clinical app (boson env)
npm run app                   # Run clinical app (boson env, with codegen watch)
npm run app:tau               # Run clinical app (local tau env)
npm nx run patient:pullenv    # Get env vars for patient app (boson env)
npm run patient               # Run patient app (boson env, with codegen watch)
npm run patient:tau           # Run patient app (local tau env)
npx nx run elements:start     # Elements dev server at localhost:3000 (no hot reload)
```

### Linting

```bash
npm run lint             # Lint all projects
npm run lint:fix         # Fix lint + prettier issues across all projects
npx nx run app:lint      # Lint clinical app only
npx nx run patient:lint  # Lint patient app only
npx nx run elements:lint # Lint e
```

</details>
