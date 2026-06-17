---
name: chatfire-AI__huobao-drama
source: https://github.com/chatfire-AI/huobao-drama/blob/d06eb385c62cde7c70fb6e1b921c729e77e7fbf8/CLAUDE.md
repo: chatfire-AI/huobao-drama
kind: claude-md
stars: 12722
last_pushed: 2026-05-21T10:53:00Z
license: unknown
score: 8
domains: [fullstack, ai-agents, backend-api, web-frontend]
tags: [architecture-heavy, typescript, full-stack]
curated: 2026-06-15
curated_by: config-scout
---

# chatfire-AI/huobao-drama — claude-md

**Why it's worth keeping:** It includes high-level implementation patterns like state management strategies and SSE streaming, which prevents the agent from guessing how to implement features. It also provides explicit database connection details to avoid unnecessary migration errors.

**Summary:** Provides a comprehensive architectural blueprint for a full-stack AI application covering both backend and frontend logic.

**Source credibility:** High; a highly-starred, active open-source project.

**Recency:** Current; utilizes modern stacks like Vite, Hono, and Mastra.

**Source:** [chatfire-AI/huobao-drama/CLAUDE.md](https://github.com/chatfire-AI/huobao-drama/blob/d06eb385c62cde7c70fb6e1b921c729e77e7fbf8/CLAUDE.md) · 12722★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

Huobao Drama — AI-powered drama/video production tool. Full TypeScript stack.

## Structure

```
backend/   — Hono + Drizzle ORM + Mastra (AI agents) + better-sqlite3
frontend/  — Vue 3 + TypeScript + Vite (pure CSS, no UI framework)
configs/   — config.yaml
data/      — SQLite database + static files
skills/    — Agent SKILL.md definitions
```

## Commands

### Backend (`backend/`)
- `npm run dev` — Start dev server with tsx watch (port 5679)
- `npm start` — Start production server
- `npm run typecheck` — TypeScript type checking

### Frontend (`frontend/`)
- `npm run dev` — Vite dev server (port 3013, proxies /api to 5679)
- `npm run build` — Production build

## Architecture

### Backend
- **HTTP**: Hono framework with CORS, logger middleware
- **Database**: Drizzle ORM + better-sqlite3, WAL mode, schema in `src/db/schema.ts`
- **AI Agents**: Mastra framework with AI SDK (OpenAI compatible providers)
- **Agent Types**: script_rewriter, extractor, storyboard_breaker
- **SSE Streaming**: Hono streamSSE for agent chat responses
- **File Storage**: Local filesystem under `data/static/`

### Frontend
- **Vue 3** + TypeScript + Vite
- **Routing**: Vue
```

</details>
