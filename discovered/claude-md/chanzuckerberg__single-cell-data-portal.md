---
name: chanzuckerberg__single-cell-data-portal
source: https://github.com/chanzuckerberg/single-cell-data-portal/blob/e379ea61f7ea537478e7e861e95c8b55458bf89f/CLAUDE.md
repo: chanzuckerberg/single-cell-data-portal
kind: claude-md
stars: 91
last_pushed: 2026-06-13T15:48:54Z
license: mit
score: 9
domains: [full-stack, data-science, web-development]
tags: [architecture-map, command-reference, environment-setup]
curated: 2026-06-15
curated_by: config-scout
---

# chanzuckerberg/single-cell-data-portal — claude-md

**Why it's worth keeping:** Provides highly specific command groupings for different stacks and a clear directory/architecture map that enables efficient navigation.

**Summary:** A comprehensive guide for a complex full-stack application covering Python backend and Next.js frontend operations.

**Source credibility:** High; maintained by the Chan Zuckerberg Initiative with recent activity.

**Recency:** Very current, referencing modern technologies like Next.js 14 and Ruff.

**Source:** [chanzuckerberg/single-cell-data-portal/CLAUDE.md](https://github.com/chanzuckerberg/single-cell-data-portal/blob/e379ea61f7ea537478e7e861e95c8b55458bf89f/CLAUDE.md) · 91★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the CZ CELLxGENE Discover data portal - a platform for publishing, discovering and exploring single-cell datasets. It's a full-stack application with Python backend services and a Next.js frontend.

## Development Commands

### Python/Backend Commands

- `make fmt` - Auto-format Python code with black and run pre-commit hooks
- `make lint` - Run ruff linting on Python code
- `make unit-test` - Run all unit tests (equivalent to `make local-unit-test`)
- `make functional-test` - Run functional tests with pytest
- `make local-init` - Set up complete local development environment with Docker
- `make local-start` - Start existing local Docker environment
- `make local-stop` - Stop local Docker environment
- `make local-logs CONTAINER=<name>` - View logs for specific container
- `make local-shell CONTAINER=<name>` - Open shell in container
- `make local-dbconsole` - Connect to local PostgreSQL database

### Frontend Commands (run from `/frontend`)

- `npm run dev` - Start development server with HTTPS
- `npm run build` - Build production bundle
```

</details>
