---
name: juliuss007__physik
source: https://github.com/juliuss007/physik/blob/6b2ff9e7239e5f80462ac387575b268f7fa1795a/CLAUDE.md
repo: juliuss007/physik
kind: claude-md
stars: 1
last_pushed: 2026-02-13T00:17:36Z
license: unknown
score: 9
domains: [web-frontend, agents-ai, state-management]
tags: [nextjs, mcp, architectural-patterns, procedural-workflows]
curated: 2026-06-14
curated_by: config-scout
---

# juliuss007/physik — claude-md

**Why it's worth keeping:** The 'To add a [Feature]' sections provide perfect step-by-step workflows that prevent pattern drift, while the MCP integration details facilitate seamless agentic tool use.

**Summary:** A highly detailed technical manual that maps out architectural patterns, state management flows, and procedural instructions for extending specific features. It provides a deep mental model of the application to ensure AI-led changes remain consistent with existing patterns.

**Source credibility:** Low star count suggests a personal project, but the documentation quality is professional and highly structured.

**Recency:** Current; uses modern Next.js patterns and specific Model Context Protocol (MCP) integration logic.

**Source:** [juliuss007/physik/CLAUDE.md](https://github.com/juliuss007/physik/blob/6b2ff9e7239e5f80462ac387575b268f7fa1795a/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Next.js 14 App Router application for tracking physics study notes and exams. The app is **fully client-side** with local persistence using `localStorage`, featuring Markdown/LaTeX rendering, PDF export, and FullCalendar integration. All state is managed via React Context + Reducers.

## Development Commands

```bash
# Install dependencies
npm install

# Development server (localhost:3000)
npm run dev

# Production build
npm run build

# Start production server
npm run start

# Lint with ESLint
npm run lint

# Test MCP tools via Streamable HTTP
node scripts/mcp-test.mjs http://localhost:3000/api/mcp
```

## Architecture

### State Management Pattern

The app uses a **Context + Reducer pattern** for all state management. There are three main state providers:

1. **NotesProvider** (`lib/notes/index.tsx`)
   - Manages all note CRUD operations
   - Automatically persists to `localStorage` key: `physik-notes`
   - Reducer actions: `create`, `update`, `delete`, `bulk-set`
   - Notes are auto-sorted by `updatedAt` (most recent first)

2. **Cal
```

</details>
