---
name: tracewayapp__traceway
source: https://github.com/tracewayapp/traceway/blob/fdb812eea8e9dbe5328da08cd71b84cf551d1c8b/CLAUDE.md
repo: tracewayapp/traceway
kind: claude-md
stars: 855
last_pushed: 2026-06-15T04:07:04Z
license: mit
score: 9
domains: [backend-api, web-frontend, go-lang, database-orm]
tags: [internal-library-usage, architectural-patterns, technical-documentation]
curated: 2026-06-15
curated_by: config-scout
---

# tracewayapp/traceway — claude-md

**Why it's worth keeping:** The 'Common Pitfalls' and 'Transaction Helper' sections are excellent examples of how to prevent LLM errors with proprietary or niche libraries. It explicitly teaches the difference between middleware-based transactions and closure-based ones, which is crucial for correct state management.

**Summary:** Provides specific architectural patterns and operational instructions, focusing heavily on an internal PostgreSQL ORM (go-lightning). It includes detailed transaction management rules and UI/UX consistency guidelines.

**Source credibility:** High; a highly starred, actively maintained repository following modern development standards.

**Recency:** Very current; references cutting-edge tech like Svelte 5, Tailwind v4, and Go 1.26.

**Source:** [tracewayapp/traceway/CLAUDE.md](https://github.com/tracewayapp/traceway/blob/fdb812eea8e9dbe5328da08cd71b84cf551d1c8b/CLAUDE.md) · 855★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Traceway Project

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Traceway is an error tracking and monitoring platform consisting of:
- **Frontend**: SvelteKit 2 dashboard application with Svelte 5
- **Backend**: Go/Gin API server with ClickHouse database
- **CLI**: Go/Cobra command-line client for the backend HTTP API (`/cli`)
- **Go Client SDK**: Distributed tracing SDK for Go applications (external repo)

---

## Code Style

- **No pointless comments**: Do not add comments that simply describe what the code does. The code should be self-explanatory. Only add comments when explaining non-obvious "why" decisions.
- **No `py-4` in dialog form content**: Do not add `py-4` on the content wrapper inside `AlertDialog` or `Dialog` components — it creates too much blank space between the form and the action buttons.
- **Dialog button labels & toasts**: For form dialogs, use descriptive button labels with icons instead of generic "Create"/"Update". Create actions: `<Plus icon> {Action} {Entity}` (e.g., "+ New Widget Group"). Update actions: `<Check icon> Update {Entity}`. After successful create/up
```

</details>
