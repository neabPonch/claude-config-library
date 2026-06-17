---
name: Prismer-AI__Prismer__claude
source: https://github.com/Prismer-AI/Prismer/blob/2dbe71feebeb53e2a54c708cac676835e08c2f24/web/CLAUDE.md
repo: Prismer-AI/Prismer
kind: claude-md
stars: 782
last_pushed: 2026-06-10T04:36:23Z
license: other
score: 9
domains: [web-frontend, desktop-app, fullstack]
tags: [nextjs, tauri, zustand, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# Prismer-AI/Prismer — claude-md

**Why it's worth keeping:** It explicitly differentiates between global, layout-level, and workspace-specific state scopes, and provides critical guidance on legacy vs. v2 API patterns to prevent architectural drift.

**Summary:** Provides a comprehensive mental model of a complex Next.js and Tauri application, covering command suites, routing logic, and state management hierarchies.

**Source credibility:** Highly credible source with a significant star count (782) and high recent activity.

**Recency:** Extremely current; includes modern technologies like React 19 and Tailwind CSS 4.

**Source:** [Prismer-AI/Prismer/web/CLAUDE.md](https://github.com/Prismer-AI/Prismer/blob/2dbe71feebeb53e2a54c708cac676835e08c2f24/web/CLAUDE.md) · 782★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Prismer.AI (PISA-OS) is an open academic research operating system built with Next.js 16, React 19, and TypeScript. It covers the full research lifecycle: paper discovery, reading (PDF with OCR), data analysis (Jupyter), writing (LaTeX), and AI-assisted peer review. It also supports desktop/mobile via Tauri 2.

## Common Commands

```bash
# Development
npm run dev                  # Start Next.js dev server (port 3000)
npm run sync:server          # Start WebSocket agent/sync server (port 3456)
npm run build                # prisma generate && next build
npm run lint                 # ESLint (Next.js core-web-vitals + TypeScript rules)

# Database (SQLite for dev, MySQL for prod)
npm run db:generate          # Generate Prisma Client (output: src/generated/prisma)
npm run db:push              # Push schema to database
npm run db:migrate           # Create migration
npm run db:studio            # Open Prisma Studio GUI

# Verify external services
npm run verify:all           # Check S3, MySQL, Redis, remote connections

# Tauri (desktop/mobile)
npm
```

</details>
