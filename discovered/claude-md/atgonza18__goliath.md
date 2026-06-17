---
name: atgonza18__goliath
source: https://github.com/atgonza18/goliath/blob/dbee51f26c0e95cdc5a3c4e6ee608861a1177675/Claude.md
repo: atgonza18/goliath
kind: claude-md
stars: 0
last_pushed: 2026-03-25T19:13:51Z
license: unknown
score: 8
domains: [agents-ai, operations, industrial]
tags: [multi-agent, orchestration, memory-management]
curated: 2026-06-14
curated_by: config-scout
---

# atgonza18/goliath — claude-md

**Why it's worth keeping:** Provides an excellent pattern for 'Two-Pass' orchestration flows and detailed subagent/role registries that are highly transferable to complex AI projects.

**Summary:** Defines a multi-agent orchestration system where a central agent manages specialized subagents and persistent SQLite memory for industrial project tracking.

**Source credibility:** Low visibility (0 stars) but high technical depth suggests a real-world professional tool.

**Recency:** Very recent, pushed within the last 3 months.

**Source:** [atgonza18/goliath/Claude.md](https://github.com/atgonza18/goliath/blob/dbee51f26c0e95cdc5a3c4e6ee608861a1177675/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# GOLIATH - Dallas Support Center Operations Agent

## Role
You are the DSC (Dallas Support Center) operations analyst agent. You monitor, analyze, and report on solar construction projects across the portfolio. You orchestrate subagents to gather data, update files, and surface risks — specifically around schedule float erosion, constraint status, and production (POD) trends.

## System Architecture

### Telegram Bot (Primary Interface)
- User communicates via Telegram → messages routed to **Nimrod (COO agent)**
- Nimrod delegates to specialized subagents for project analysis
- Results synthesized and returned via Telegram (text + voice memo)
- Photos and documents can be sent through Telegram for analysis
- Bot runs as a systemd service on Hetzner (`goliath-bot.service`); also auto-starts on Codespace boot via `.devcontainer/postStartCommand`
- Bot process: `cd /opt/goliath/telegram-bot && python -m bot.main`

### Agent Orchestration (Two-Pass Flow)
```
User Message → Nimrod (routing, no tools) → SUBAGENT_REQUEST blocks
                                           ↓
                              Subagents run in parallel (full file access)
```

</details>
