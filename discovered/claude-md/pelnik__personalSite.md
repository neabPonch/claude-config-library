---
name: pelnik__personalSite
source: https://github.com/pelnik/personalSite/blob/3b05ad6bda1b4a63c3efa93dd6a2e689b38c8e48/claude.md
repo: pelnik/personalSite
kind: claude-md
stars: 0
last_pushed: 2026-03-17T22:45:32Z
license: unknown
score: 9
domains: [fullstack, web-development, devops]
tags: [monorepo, express, react, postgresql, deployment-aware]
curated: 2026-06-14
curated_by: config-scout
---

# pelnik/personalSite — claude-md

**Why it's worth keeping:** Includes critical operational 'gotchas' like hardware limitations (EC2 memory) and provides specific coding standards for error handling and database patterns.

**Summary:** A high-density guide for a full-stack React/Express monorepo covering architecture, environment configuration, and deployment constraints.

**Source credibility:** Personal portfolio project demonstrating high-quality documentation practices by a single developer.

**Recency:** Very current, mentioning React 19 and modern Node.js environments.

**Source:** [pelnik/personalSite/claude.md](https://github.com/pelnik/personalSite/blob/3b05ad6bda1b4a63c3efa93dd6a2e689b38c8e48/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — personalSite

## Project Overview

This is Matt Pelnik's personal portfolio site and full-stack application showcase. It is a React + Express monorepo: the Express server serves the compiled React frontend as static files and also exposes several REST APIs for portfolio projects.

The site is deployed on an EC2 instance (Ubuntu, managed with PM2) and uses GitHub Actions for CI/CD — tests run on every PR, and merges to `main` automatically build the React app on GitHub's servers and deploy it to EC2 via rsync + SSH.

---

## Architecture

### Server

`server.js` at the project root is the Express entry point. It:
- Serves `build/` as static files (the compiled React app)
- Mounts all API routes under `/api`
- Falls back to `build/index.html` for all other routes (SPA behavior)
- Runs HTTP on port 80 (dev: 3000) and HTTPS on port 443 (dev: 3443) when SSL certs are present in `Keys/`

### Frontend

React 19 SPA with TypeScript. Entry point is `src/index.tsx`. Components live in `src/components/`, organized by feature. There are also three full embedded React applications in `src/fullReactProjects/` (FitnessTrackerFrontEnd, juicebox, stranger) that are portfolio demos.

#
```

</details>
