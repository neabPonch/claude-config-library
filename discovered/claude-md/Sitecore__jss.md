---
name: Sitecore__jss
source: https://github.com/Sitecore/jss/blob/049c5ba1c4c0d218960c78bda51667f2d258e2c6/CLAUDE.md
repo: Sitecore/jss
kind: claude-md
stars: 274
last_pushed: 2026-06-09T14:52:23Z
license: apache-2.0
score: 9
domains: [web-frontend, monorepo, typescript-sdk]
tags: [monorepo, architectural-intent, enterprise-scale]
curated: 2026-06-14
curated_by: config-scout
---

# Sitecore/jss — claude-md

**Why it's worth keeping:** The 'Vibe-Coding Principles' section provides excellent meta-instructions for engineering philosophy, while the explicit package/directory mapping is perfect for navigating large codebases.

**Summary:** A highly detailed guide for a complex TypeScript monorepo that defines architectural intent and structural navigation.

**Source credibility:** High; Sitecore is a major enterprise entity with an actively maintained open-source repository.

**Recency:** Very current; references modern Node LTS versions and contemporary development workflows.

**Source:** [Sitecore/jss/CLAUDE.md](https://github.com/Sitecore/jss/blob/049c5ba1c4c0d218960c78bda51667f2d258e2c6/CLAUDE.md) · 274★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Agent Guide for Sitecore JavaScript Services (JSS)

## Project Overview

This is **Sitecore JavaScript Services (JSS)** — a TypeScript/JavaScript SDK for building modern web applications with Sitecore XM Cloud and on-premises. The project provides core layout/GraphQL functionality, React/Angular/Vue/Next.js integrations, and CLI tools for scaffolding applications.

### Tech Stack
- **Language**: TypeScript (Node LTS)
- **Runtime**: Node LTS (>=24)
- **Build**: `tsc` → `dist/`, templates built via `scripts/build-templates.ts` in create-sitecore-jss
- **Testing**: Mocha + Sinon + Chai, coverage via `nyc`
- **Lint/format**: ESLint + Prettier
- **Package Manager**: Yarn 4.12.0

### Core Packages
- `@sitecore-jss/sitecore-jss` - Core SDK (layout, GraphQL, i18n, tracking, editing)
- `@sitecore-jss/sitecore-jss-react` - React components (Text, Image, Link, Placeholder)
- `@sitecore-jss/sitecore-jss-nextjs` - Next.js integration and middleware
- `@sitecore-jss/sitecore-jss-angular` - Angular integration
- `@sitecore-jss/sitecore-jss-vue` - Vue integration
- `@sitecore-jss/sitecore-jss-cli` - CLI (jss deploy, jss setup)
- `create-sitecore-jss` - Scaffolding CLI and templates
```

</details>
