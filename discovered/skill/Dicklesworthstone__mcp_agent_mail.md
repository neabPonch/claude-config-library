---
name: Dicklesworthstone__mcp_agent_mail
source: https://github.com/Dicklesworthstone/mcp_agent_mail/blob/b18d925c3e303a13f031fccb6c21eb6c2b318b9c/SKILL.md
repo: Dicklesworthstone/mcp_agent_mail
kind: skill
stars: 1984
last_pushed: 2026-06-13T17:19:56Z
license: other
score: 9
domains: [agents-ai, cli-tools, workflow-orchestration]
tags: [mcp, multi-agent, coordination, file-locking]
curated: 2026-06-16
curated_by: config-scout
---

# Dicklesworthstone/mcp_agent_mail — skill

**Why it's worth keeping:** The advisory file reservation system coupled with a pre-commit guard is a brilliant mechanism for preventing race conditions in agentic environments. The 'macro' pattern for single-call session bootstrapping significantly reduces the cognitive and token overhead of starting new workstreams.

**Summary:** An asynchronous coordination layer that provides multi-agent workflows with shared identities, threaded messaging, and file reservation leases to prevent write conflicts.

**Source credibility:** High: highly starred (1984) and actively maintained project.

**Recency:** Current; utilizes modern FastMCP standards and is designed for today's agentic ecosystems.

**Source:** [Dicklesworthstone/mcp_agent_mail/SKILL.md](https://github.com/Dicklesworthstone/mcp_agent_mail/blob/b18d925c3e303a13f031fccb6c21eb6c2b318b9c/SKILL.md) · 1984★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: agent-mail
description: "MCP Agent Mail - Mail-like coordination layer for multi-agent workflows. Identities, inbox/outbox, file reservations, contact policies, threaded messaging, pre-commit guard, Human Overseer, static exports, disaster recovery. Git+SQLite backed. Python/FastMCP."
---

# MCP Agent Mail

A mail-like coordination layer for coding agents exposed as an HTTP-only FastMCP server. Provides memorable identities, inbox/outbox, file reservation leases, contact policies, searchable message history, and Human Overseer messaging. Backed by Git (human-auditable artifacts) and SQLite (fast queries with FTS5).

## Why This Exists

Without coordination, multiple agents:
- Overwrite each other's edits or panic on unexpected diffs
- Miss critical context from parallel workstreams
- Require humans to relay messages between tools

Agent Mail solves this with:
- Memorable identities (adjective+noun names like "GreenCastle")
- Advisory file reservations to signal editing intent
- Threaded messaging with importance levels and acknowledgments
- Pre-commit guard to enforce reservations at commit time
- Human Overseer for direct human-to-agent communication

## Starting the Ser
```

</details>
