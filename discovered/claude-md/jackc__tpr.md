---
name: jackc__tpr
source: https://github.com/jackc/tpr/blob/0de68ee3f367b28fad8fd565b69d6b73013434fb/CLAUDE.md
repo: jackc/tpr
kind: claude-md
stars: 25
last_pushed: 2026-03-24T12:19:26Z
license: unknown
score: 9
domains: [backend-api, web-frontend, go, svelte]
tags: [architecture-diagram, implementation-recipes, fullstack]
curated: 2026-06-15
curated_by: config-scout
---

# jackc/tpr — claude-md

**Why it's worth keeping:** The inclusion of 'Common Tasks' provides exact implementation recipes, while the ASCII diagram clarifies dependency injection through custom handler types.

**Summary:** Provides a highly structured blueprint of the project's architecture, specific coding patterns, and operational workflows.

**Source credibility:** High; written by a solo developer for a functional real-world tool with specific, non-generic technical details.

**Recency:** Highly current; explicitly mentions Svelte 5 and modern Go patterns.

**Source:** [jackc/tpr/CLAUDE.md](https://github.com/jackc/tpr/blob/0de68ee3f367b28fad8fd565b69d6b73013434fb/CLAUDE.md) · 25★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - AI Assistant Context

This document provides context for AI assistants (like Claude) working with The Pithy Reader codebase.

## Project Overview

**The Pithy Reader** is a self-hosted RSS/Atom feed aggregator built with Go and Svelte. It allows users to subscribe to feeds, automatically fetches updates, and provides a keyboard-driven interface for reading articles.

**Version**: 0.8.1
**Author**: Jack Christensen
**License**: Copyright Jack Christensen

## Architecture

### High-Level Design

```
┌─────────────┐     HTTP/JSON     ┌──────────────┐
│   Svelte    │ ←──────────────→  │   Go HTTP    │
│   Frontend  │      /api/*       │   Server     │
│  (SvelteKit)│                   │   (chi)      │
└─────────────┘                   └──────┬───────┘
                                         │
                      ┌──────────────────┼──────────────────┐
                      ▼                  ▼                  ▼
                ┌───────────┐     ┌─────────────┐   ┌──────────┐
                │ PostgreSQL│     │ Feed Updater│   │  SMTP    │
                │  Database │     │ (Background)│   │  Mailer  │
                └───────────┘     └─────────────┘   └──────────┘
`
```

</details>
