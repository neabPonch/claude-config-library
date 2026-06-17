---
name: Sherlockouo__music
source: https://github.com/Sherlockouo/music/blob/0e1c8dc7d3a6361ee7a9cf66a46e047594dc6fbb/CLAUDE.md
repo: Sherlockouo/music
kind: claude-md
stars: 692
last_pushed: 2026-05-27T03:48:18Z
license: agpl-3.0
score: 9
domains: [desktop-app, monorepo, electron]
tags: [pnpm, turborepo, ipc, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# Sherlockouo/music — claude-md

**Why it's worth keeping:** Includes specific procedural workflows (e.g., adding new IPC channels) that tell the agent exactly which files to modify in what order. It also clearly maps out cross-process communication paths between Main/Renderer processes.

**Summary:** Comprehensive guide for a complex Electron/React monorepo detailing command filtering, IPC communication patterns, and state management locations.

**Source credibility:** High-quality, popular open-source project with significant stars and recent activity.

**Recency:** Extremely current; last pushed within the past month.

**Source:** [Sherlockouo/music/CLAUDE.md](https://github.com/Sherlockouo/music/blob/0e1c8dc7d3a6361ee7a9cf66a46e047594dc6fbb/CLAUDE.md) · 692★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

R3PLAYX is a third-party NetEase Cloud Music player built with React + Electron. It's a cross-platform desktop application that also has a web version. The project uses a monorepo architecture with Turborepo for build orchestration.

**Key Technologies:**
- **Desktop:** Electron 28, React 18, Fastify (local server), better-sqlite3
- **Web:** React 18, Vite 4, Tailwind CSS, Framer Motion
- **Server:** Fastify 4, Prisma, SQLite
- **Build:** Turborepo, PNPM workspaces

## Development Setup

### Prerequisites
- Node.js >= 16.0.0 (v18.12.1 recommended)
- PNPM package manager (v8.6.12)

### Initial Setup
```bash
# Install pnpm (if not already installed)
npm i -g pnpm

# Set electron mirror (for China users)
pnpm config set electron_mirror=https://repo.huaweicloud.com/electron/

# Copy environment files
cp .env.example .env

# Install dependencies (runs post-install scripts automatically)
pnpm install
```

**Important:** The root `pnpm install` automatically runs `post-install` scripts in parallel, which:
- Builds SQLite binaries for desktop (better-sql
```

</details>
