---
name: multica-ai__multica
source: https://github.com/multica-ai/multica/blob/f2e72577b2fa95302692aa54d546d7ac4d627b99/CLAUDE.md
repo: multica-ai/multica
kind: claude-md
stars: 36724
last_pushed: 2026-06-15T11:50:49Z
license: other
score: 9
domains: [monorepo, fullstack, architecture]
tags: [monorepo, state-management, architectural-guardrails]
curated: 2026-06-15
curated_by: config-scout
---

# multica-ai/multica — claude-md

**Why it's worth keeping:** It uses 'Hard Rules' and 'Footguns' sections to prevent common LLM mistakes; provides clear dependency direction and state ownership logic.

**Summary:** An exceptional architectural blueprint for a complex Go/TypeScript monorepo that defines strict boundaries for state management and cross-platform sharing.

**Source credibility:** High; high-star repository with very recent activity.

**Recency:** Current; highly relevant for modern monorepo/agentic workflows.

**Source:** [multica-ai/multica/CLAUDE.md](https://github.com/multica-ai/multica/blob/f2e72577b2fa95302692aa54d546d7ac4d627b99/CLAUDE.md) · 36724★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Conventions reference

The single source of truth for **code naming, the i18n translation glossary, and the Chinese voice guide** is the docs site:

- **`apps/docs/content/docs/developers/conventions.mdx`** (English)
- **`apps/docs/content/docs/developers/conventions.zh.mdx`** (Chinese)

Read that page before:

- Writing or editing translations (`packages/views/locales/`)
- Naming a new route, package, file, DB column, or TS type
- Writing Chinese product copy (UI strings, error messages, docs)

The legacy `packages/views/locales/glossary.md` is now a stub redirecting to the docs page; do not rely on it.

## Project Context

Multica is an AI-native task management platform — like Linear, but with AI agents as first-class citizens.

- Agents can be assigned issues, create issues, comment, and change status
- Supports local (daemon) and cloud agent runtimes
- Built for 2-10 person AI-native teams

## Architecture

**Go backend + monorepo frontend (pnpm workspaces + Turborepo) with shared packages.**

- `server/` — Go backend (Chi router, sqlc for DB, gorilla/websock
```

</details>
