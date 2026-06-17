---
name: opennem__opennem-fe
source: https://github.com/opennem/opennem-fe/blob/d6787b4fc53b58d77d57e0fd18d83c6fd0879ccf/CLAUDE.md
repo: opennem/opennem-fe
kind: claude-md
stars: 78
last_pushed: 2026-05-12T06:25:11Z
license: mit
score: 7
domains: [web-frontend]
tags: [nuxt, vue, legacy-environment, docker]
curated: 2026-06-15
curated_by: config-scout
---

# opennem/opennem-fe — claude-md

**Why it's worth keeping:** Effectively prevents environment-related errors by detailing strict Node/Yarn version requirements and providing Docker command alternatives to ensure build stability.

**Summary:** Provides critical environmental constraints and structural overview for a legacy Nuxt.js application.

**Source credibility:** Established open-source project with recent maintenance activity.

**Recency:** Highly relevant for current agents navigating legacy or specific environment constraints.

**Source:** [opennem/opennem-fe/CLAUDE.md](https://github.com/opennem/opennem-fe/blob/d6787b4fc53b58d77d57e0fd18d83c6fd0879ccf/CLAUDE.md) · 78★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# OpenNEM Frontend - Project Context

## About
OpenNEM is an open platform for Australian National Electricity Market data visualization. This Vue.js/Nuxt.js frontend displays interactive charts and maps for power generation, emissions, and market data across Australia.

## Technology Stack
- **Framework**: Nuxt.js 2 (Vue.js framework) 
- **Charts**: D3.js for data visualizations
- **Maps**: Mapbox GL for facility mapping
- **Styling**: Bulma CSS framework + custom SCSS
- **Package Manager**: Yarn (v1 classic)

## Requirements
- **Node.js**: v14 (does not support versions above v14)
- **Yarn**: v1 (classic) required for package management

## Development Commands

### Native (requires Node.js v14)
```bash
# Install dependencies
yarn install

# Start development server
yarn dev

# Build for production
yarn build

# Generate static site
yarn generate

# Lint code
yarn lint

# Fix linting issues
yarn fix
```

### Docker (recommended - isolates Node.js v14)
```bash
# Build and start development server
docker-compose up --build

# Run commands in container
docker-compose exec opennem-fe yarn install
docker-compose exec opennem-fe yarn lint
docker-compose exec opennem-fe yarn build

# St
```

</details>
