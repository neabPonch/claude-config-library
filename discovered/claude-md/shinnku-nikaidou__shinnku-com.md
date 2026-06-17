---
name: shinnku-nikaidou__shinnku-com
source: https://github.com/shinnku-nikaidou/shinnku-com/blob/07990d66561a58ec71418901ac659efcca07a284/CLAUDE.md
repo: shinnku-nikaidou/shinnku-com
kind: claude-md
stars: 628
last_pushed: 2026-06-01T08:51:28Z
license: mit
score: 9
domains: [web-frontend, backend-api, ai-service, monorepo]
tags: [nextjs, rust, python, monorepo]
curated: 2026-06-15
curated_by: config-scout
---

# shinnku-nikaidou/shinnku-com — claude-md

**Why it's worth keeping:** The 'Development Commands' section is exceptionally useful for agents to avoid tool-execution errors; the architecture breakdown provides necessary context for cross-service logic.

**Summary:** A highly structured guide for a polyglot monorepo containing Next.js, Rust (Axum), and Python AI components. It effectively maps out specific development workflows and architectural dependencies across different stacks.

**Source credibility:** High-quality signal from a well-starred repository with recent maintenance.

**Recency:** Very current, utilizing modern tech like Next.js 15 and uv/Python tools.

**Source:** [shinnku-nikaidou/shinnku-com/CLAUDE.md](https://github.com/shinnku-nikaidou/shinnku-com/blob/07990d66561a58ec71418901ac659efcca07a284/CLAUDE.md) · 628★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Shinnku-com is a monorepo containing a galgame resource website with three main components:

- **Frontend**: Next.js 15 app with TypeScript, Tailwind CSS, and MDX support
- **Backend**: Rust web service using Axum framework with Redis integration
- **AI**: Python-based AI service using Falcon ASGI with LangChain and ChromaDB

## Development Commands

### Frontend (in `frontend/` directory)

- **Dev server**: `pnpm run dev` (uses Turbopack)
- **Build**: `pnpm run build`
- **Lint**: `pnpm run lint` (ESLint with TypeScript)
- **Format**: `pnpm run format` (Prettier)

### Backend (in `backend/` directory)

- **Run server**: `cargo run -p server`
- **Build**: `cargo build`
- **Test**: `cargo test`
- **Format**: `cargo fmt`
- **Lint**: `cargo clippy` (uses strict Clippy rules from Cargo.toml)

### AI Service (in root directory)

- **Install dependencies**: `uv sync` or `pip install -r requirements.txt`
- **Run AI service**: `python -m ai.serve` or `shinnku-ai-serve`
- **Format**: `black ai/` and `isort ai/`
- **Test**: `pytest` (with coverage via `pyte
```

</details>
