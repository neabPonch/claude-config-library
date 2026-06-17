---
name: dandaka__traul
source: https://github.com/dandaka/traul/blob/4de8dc81b1ee29a1f8fbfd3266d9ba805bcc9f1c/skill.md
repo: dandaka/traul
kind: skill
stars: 110
last_pushed: 2026-05-06T16:26:41Z
license: agpl-3.0
score: 8
domains: [cli-tools, agents-ai, information-retrieval]
tags: [personal-intelligence, search, hybrid-search, sync]
curated: 2026-06-14
curated_by: config-scout
---

# dandaka/traul — skill

**Why it's worth keeping:** Provides highly specific guidance on choosing between search modes (semantic vs. FTS) and uses a 'signals' system to surface actionable insights rather than just raw data.

**Summary:** A personal intelligence engine that indexes communication streams (Slack, Gmail, etc.) for hybrid semantic and keyword search.

**Source credibility:** Legitimate open-source tool with 110 stars and recent activity.

**Recency:** Extremely current; specifically includes Claude Code session extraction as a core feature.

**Source:** [dandaka/traul/skill.md](https://github.com/dandaka/traul/blob/4de8dc81b1ee29a1f8fbfd3266d9ba805bcc9f1c/skill.md) · 110★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: traul
description: Personal Intelligence Engine CLI for syncing, searching, and monitoring messages from Slack, Telegram, Discord, Linear, Gmail, Claude Code sessions, Markdown files, and WhatsApp. Use when working with traul commands, message sync, search, signals, briefings, or browsing chat history.
allowed-tools:
  - Bash
  - Read
  - Edit
  - Write
  - Glob
  - Grep
---

# Traul — Personal Intelligence Engine

CLI tool that watches communication streams (Slack, Telegram, Discord, Linear, Gmail, Claude Code sessions, Markdown files, WhatsApp), indexes messages, detects patterns via signals, and surfaces actionable insights.

**Runtime:** Bun + TypeScript | **DB:** SQLite (WAL mode, FTS5, sqlite-vec) | **Embeddings:** node-llama-cpp (Qwen3-Embedding-0.6B), Ollama fallback | **Version:** 0.2.0

**Project:** `/Users/dandaka/projects/traul`

---

## CLI Commands

### `traul sync [source]`

Sync messages from communication sources incrementally.

| Argument | Description |
|----------|-------------|
| `source` | Optional. `slack`, `telegram`, `discord`, `linear`, `gmail`, `claudecode`, `markdown`, or `whatsapp`. Omit to sync all. |

- Uses cursor-based incremental sync (on
```

</details>
