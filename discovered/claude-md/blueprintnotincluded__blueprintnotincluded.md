---
name: blueprintnotincluded__blueprintnotincluded
source: https://github.com/blueprintnotincluded/blueprintnotincluded/blob/d5feeb7aa54f78b5acb02db0c8c286d0106ec3b9/CLAUDE.md
repo: blueprintnotincluded/blueprintnotincluded
kind: claude-md
stars: 31
last_pushed: 2026-06-15T03:36:17Z
license: mit
score: 9
domains: [fullstack, web-dev, devops, security]
tags: [typescript, express, angular, mongodb, github-cli]
curated: 2026-06-15
curated_by: config-scout
---

# blueprintnotincluded/blueprintnotincluded — claude-md

**Why it's worth keeping:** It uses 'negative constraints' to prevent dependency bloat (e.g., 'do not introduce Jest') and includes a detailed `gh` CLI section to empower agentic autonomy in CI/CD tasks.

**Summary:** A comprehensive full-stack instruction set covering architecture, specific toolchains, and rigorous environmental constraints.

**Source credibility:** High-quality, highly specific documentation for an active full-stack project.

**Recency:** Very current; mentions modern versions of Node, Angular, and TypeScript.

**Source:** [blueprintnotincluded/blueprintnotincluded/CLAUDE.md](https://github.com/blueprintnotincluded/blueprintnotincluded/blob/d5feeb7aa54f78b5acb02db0c8c286d0106ec3b9/CLAUDE.md) · 31★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the source repository for blueprintnotincluded.org, a web application for creating and sharing blueprints for the game Oxygen Not Included. It's a full-stack TypeScript application with an Express.js backend and Angular frontend.

## Architecture

- **Backend**: Express.js with TypeScript (`app/` directory)
  - Main server entry: `app/server.ts`
  - API routes in `app/api/`
  - MongoDB with Mongoose for data persistence
  - JWT authentication for user sessions
  - Blueprint processing and image generation using Canvas and PIXI.js
  - Batch processing scripts for assets in `app/api/batch/`
  
- **Frontend**: Angular application (`frontend/` directory)
  - Blueprint visualization and editing interface
  - Multi-language support (English, Chinese, Russian, Korean)
  - Uses PrimeNG components

- **Shared Library**: TypeScript library (`lib/` directory)
  - Blueprint data structures and utilities
  - Drawing and rendering helpers
  - Shared between frontend and backend

## Development Commands

### Development (Recommended)
- `./dev-setup.sh`
```

</details>
