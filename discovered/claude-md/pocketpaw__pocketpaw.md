---
name: pocketpaw__pocketpaw
source: https://github.com/pocketpaw/pocketpaw/blob/3d881a7e466295020598f0154e884a0a34890185/CLAUDE.md
repo: pocketpaw/pocketpaw
kind: claude-md
stars: 857
last_pushed: 2026-06-15T17:19:04Z
license: mit
score: 9
domains: [agents-ai, cli-tools, backend-api]
tags: [knowledge-base-integration, command-reference, architecture-mapping]
curated: 2026-06-15
curated_by: config-scout
---

# pocketpaw/pocketpaw — claude-md

**Why it's worth keeping:** The 'Knowledge Base' section teaches the AI how to query documentation before modifying code; the extensive command list provides an exhaustive toolbelt for all development phases.

**Summary:** Provides deep architectural context for a multi-agent system and includes instructions for interacting with an auto-generated knowledge base.

**Source credibility:** High credibility with 857 stars and active maintenance.

**Recency:** 

**Source:** [pocketpaw/pocketpaw/CLAUDE.md](https://github.com/pocketpaw/pocketpaw/blob/3d881a7e466295020598f0154e884a0a34890185/CLAUDE.md) · 857★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

PocketPaw is a self-hosted AI agent that runs locally and is controlled via Telegram, Discord, Slack, WhatsApp, or a web dashboard. The Python package is named `pocketpaw` (the internal/legacy name), while the public-facing name is `pocketpaw`. Python 3.11+ required.

## Knowledge Base

A codebase wiki lives at `docs/wiki/` — auto-generated from AST analysis + LLM compilation. **Read the relevant wiki article before modifying a module.**

```bash
# Search the KB from terminal
cd /path/to/knowledge-base && kb search "GroupService" --scope paw-cloud

# Show a specific module's wiki
kb show group_service --scope paw-cloud

# Rebuild after big changes (also runs automatically via PostCommit hook)
kb build ./ee/cloud --scope paw-cloud --output docs/wiki/

# Check wiki health
kb lint --scope paw-cloud
```

Key wiki articles for the enterprise cloud module:
- `docs/wiki/index.md` — Full index with all articles
- `docs/wiki/group_service.md` — Chat group CRUD, membership, agents
- `docs/wiki/message_service.md` — Message CRUD, reactions, threads
- `docs/
```

</details>
