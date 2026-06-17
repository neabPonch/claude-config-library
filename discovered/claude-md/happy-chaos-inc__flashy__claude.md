---
name: happy-chaos-inc__flashy__claude
source: https://github.com/happy-chaos-inc/flashy/blob/f4636a6b1e974a734e31593ce0218cb223568e8b/flashy/CLAUDE.md
repo: happy-chaos-inc/flashy
kind: claude-md
stars: 1
last_pushed: 2026-05-31T03:22:26Z
license: unknown
score: 8
domains: [web-frontend, fullstack-dev]
tags: [autonomy, infrastructure-setup, agentic-rules]
curated: 2026-06-16
curated_by: config-scout
---

# happy-chaos-inc/flashy — claude-md

**Why it's worth keeping:** The 'Rules' section provides a blueprint for high-agency behavior (autonomy in terminal operations) and demonstrates how to use tool calls rather than plain text to trigger external notification hooks.

**Summary:** Combines deep architectural context and infrastructure setup checklists with highly specific agent behavioral instructions.

**Source credibility:** Low star count, but the content is highly specific and shows advanced understanding of agentic workflows.

**Recency:** Current; uses modern patterns for instructing autonomous code agents.

**Source:** [happy-chaos-inc/flashy/flashy/CLAUDE.md](https://github.com/happy-chaos-inc/flashy/blob/f4636a6b1e974a734e31593ce0218cb223568e8b/flashy/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

Flashy is a collaborative WYSIWYG document editor built with React, TypeScript, and Yjs CRDTs. It uses Supabase for backend persistence and real-time sync, and deploys to GitHub Pages.

## Key Commands

- `npm start` — Start dev server
- `npm test` — Run tests (Jest + React Testing Library)
- `npm run build` — Production build
- `npm run build:prod` — Production build with production env
- `npm run deploy` — Deploy to GitHub Pages

## Architecture

- **Editor**: TipTap (ProseMirror) + CodeMirror with Yjs CRDT bindings
- **State sync**: Yjs documents with y-indexeddb for offline, Supabase for persistence
- **RAG pipeline**: pgvector hybrid search (dense + sparse + RRF), OpenAI text-embedding-3-small
- **Multi-chat**: Per-thread Yjs structures (Y.Array per thread, Y.Map for thread metadata)
- **Routing**: React Router (SPA with 404.html redirect for GitHub Pages)
- **Styling**: Plain CSS

## Project Structure

- `src/pages/` — Page-level components (EditorPage, LandingPage)
- `src/components/` — Reusable UI components
- `src/hooks/` — Custom React hooks
- `src/lib/` — Library code (Supabase client, CRDT utilities)
- `src/config/` — App configuration
```

</details>
