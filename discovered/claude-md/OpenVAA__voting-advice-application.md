---
name: OpenVAA__voting-advice-application
source: https://github.com/OpenVAA/voting-advice-application/blob/9e0399286dfa269d23741b0b7829facbd084a971/CLAUDE.md
repo: OpenVAA/voting-advice-application
kind: claude-md
stars: 20
last_pushed: 2026-06-14T08:27:15Z
license: gpl-3.0
score: 9
domains: [monorepo, web-frontend, backend-api, fullstack]
tags: [monorepo, typescript, docker, sveltekit, strapi]
curated: 2026-06-15
curated_by: config-scout
---

# OpenVAA/voting-advice-application — claude-md

**Why it's worth keeping:** It explains critical build-order dependencies in the monorepo, clarifies data model philosophy to prevent logical errors, and provides specific commands for granular workspace testing.

**Summary:** A highly detailed guide for navigating a complex monorepo containing SvelteKit, Strapi, and shared logic packages.

**Source credibility:** Strong; active project with a clear, complex architecture that justifies this level of detail.

**Recency:** Very recent/current, utilizing modern toolchains like Yarn 4 and SvelteKit 2.

**Source:** [OpenVAA/voting-advice-application/CLAUDE.md](https://github.com/OpenVAA/voting-advice-application/blob/9e0399286dfa269d23741b0b7829facbd084a971/CLAUDE.md) · 20★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

OpenVAA is a framework for building Voting Advice Applications (VAAs). It's a monorepo containing frontend (SvelteKit), backend (Strapi CMS), and shared packages for matching algorithms, filters, and data management.

## Development Commands

### Setup

```bash
yarn install                    # Install all workspace dependencies
yarn dev                        # Start full Docker stack (frontend, backend, postgres, localstack)
yarn dev:down                   # Clean shutdown (removes containers, volumes, images)
yarn dev:stop                   # Stop without removing volumes
```

### Building

```bash
yarn build:app-shared          # Build @openvaa/app-shared (required before most dev work)
yarn build:shared              # Build all packages in /packages
```

### Testing

```bash
yarn test:unit                 # Run all unit tests (vitest)
yarn test:unit:watch          # Run unit tests in watch mode
yarn test:e2e                 # Run Playwright E2E tests (requires yarn dev running)
yarn playwright install       # Install Playwright browsers
```

### Lin
```

</details>
