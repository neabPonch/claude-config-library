---
name: arturdzivia-jpg__movie-watchlist
source: https://github.com/arturdzivia-jpg/movie-watchlist/blob/d9d609fdfd0539d70b5225937579e2c230bcd767/claude.md
repo: arturdzivia-jpg/movie-watchlist
kind: claude-md
stars: 0
last_pushed: 2026-02-14T23:43:44Z
license: unknown
score: 9
domains: [web-development, full-stack, api-design]
tags: [schema-documentation, deployment-warnings, workflow-templates]
curated: 2026-06-16
curated_by: config-scout
---

# arturdzivia-jpg/movie-watchlist — claude-md

**Why it's worth keeping:** Contains critical 'anti-patterns' to avoid (e.g., don't run Prisma locally) and provides procedural templates for extending the API that ensure consistency.

**Summary:** Provides deep technical context including schema summaries, API endpoints, and specific warnings about the deployment-specific database workflow.

**Source credibility:** Low star count, but the density of specific architectural detail suggests a high-effort individual project.

**Recency:** Current; reflects modern full-stack deployment and tool-use patterns.

**Source:** [arturdzivia-jpg/movie-watchlist/claude.md](https://github.com/arturdzivia-jpg/movie-watchlist/blob/d9d609fdfd0539d70b5225937579e2c230bcd767/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Movie Watchlist - Developer Guide

> **Quick Start for Claude/AI Assistants**: This document provides comprehensive instructions for understanding, modifying, and extending the Movie Watchlist application.

> **Important**: After making code changes, always commit and push to apply them:
> ```bash
> git add <changed-files> && git commit -m "description" && git push
> ```

> **Deployment Note**: This project deploys to **Railway (backend)** and **Vercel (frontend)**. There is NO local database setup - schema changes are applied automatically on Railway deploy via `prisma db push` in the `npm start` script. Do NOT attempt to run Prisma commands locally.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Quick Start](#quick-start)
3. [Architecture Documentation](#architecture-documentation)
4. [Development Workflow](#development-workflow)
5. [Common Tasks](#common-tasks)
6. [Troubleshooting](#troubleshooting)
7. [Contributing](#contributing)

---

## Project Overview

### What This Application Does

A full-stack web application for managing movie watchlists with personalized recommendations:

- **User Features:**
  - Create account and login (JWT authentication)
  -
```

</details>
