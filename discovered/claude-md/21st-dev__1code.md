---
name: 21st-dev__1code
source: https://github.com/21st-dev/1code/blob/9f1bc76fa4372c18c565b5a4f8daf38ae3595f0e/CLAUDE.md
repo: 21st-dev/1code
kind: claude-md
stars: 5559
last_pushed: 2026-03-06T21:10:12Z
license: apache-2.0
score: 9
domains: [desktop-app, electron, ai-agents, typescript]
tags: [architecture-map, troubleshooting, pattern-guidance, meta-instructions]
curated: 2026-06-15
curated_by: config-scout
---

# 21st-dev/1code — claude-md

**Why it's worth keeping:** The 'Key Patterns' section prevents architectural drift by specifying how to handle IPC/state, while the 'OpenSpec' block creates a hierarchy of authority for planning-heavy tasks.

**Summary:** Provides comprehensive architectural maps, specific tech patterns (tRPC/State), and crucial debugging workflows for a complex Electron environment.

**Source credibility:** High; high star count and professional repository structure indicate expert authorship.

**Recency:** Highly current, featuring React 19 and modern toolchain (Bun/Drizzle).

**Source:** [21st-dev/1code/CLAUDE.md](https://github.com/21st-dev/1code/blob/9f1bc76fa4372c18c565b5a4f8daf38ae3595f0e/CLAUDE.md) · 5559★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
<!-- OPENSPEC:START -->
# OpenSpec Instructions

These instructions are for AI assistants working in this project.

Always open `@/openspec/AGENTS.md` when the request:
- Mentions planning or proposals (words like proposal, spec, change, plan)
- Introduces new capabilities, breaking changes, architecture shifts, or big performance/security work
- Sounds ambiguous and you need the authoritative spec before coding

Use `@/openspec/AGENTS.md` to learn:
- How to create and apply change proposals
- Spec format and conventions
- Project structure and guidelines

Keep this managed block so 'openspec update' can refresh the instructions.

<!-- OPENSPEC:END -->

# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What is this?

**21st Agents** - A local-first Electron desktop app for AI-powered code assistance. Users create chat sessions linked to local project folders, interact with Claude in Plan or Agent mode, and see real-time tool execution (bash, file edits, web search, etc.).

## Commands

```bash
# Development
bun run dev              # Start Electron with hot reload

# Build
bun run build            # Compile app
b
```

</details>
