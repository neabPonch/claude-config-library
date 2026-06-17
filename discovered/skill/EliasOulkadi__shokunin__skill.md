---
name: EliasOulkadi__shokunin__skill
source: https://github.com/EliasOulkadi/shokunin/blob/a0f4a5f5799ecff51046988270c97152cbd0edb8/.pack/skills/memory/SKILL.md
repo: EliasOulkadi/shokunin
kind: skill
stars: 96
last_pushed: 2026-06-15T02:25:11Z
license: mit
score: 9
domains: [agents-ai, cli-tools, database]
tags: [memory, chromadb, mcp, persistent-state]
curated: 2026-06-15
curated_by: config-scout
---

# EliasOulkadi/shokunin — skill

**Why it's worth keeping:** The inclusion of detailed anti-patterns and error-handling guides prevents common failures like database flooding or context loss. It also offers specific technical patterns for high-performance embedding management and batching.

**Summary:** Provides a structured protocol for managing long-term agent memory via ChromaDB vector search across different sessions.

**Source credibility:** Strong; a specialized, active repository with solid social proof via star count.

**Recency:** Current; aligns perfectly with modern MCP-driven agent workflows used by Claude Code and Cursor.

**Source:** [EliasOulkadi/shokunin/.pack/skills/memory/SKILL.md](https://github.com/EliasOulkadi/shokunin/blob/a0f4a5f5799ecff51046988270c97152cbd0edb8/.pack/skills/memory/SKILL.md) · 96★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: memory
description: Persistent memory across AI sessions using ChromaDB vector database. Stores and retrieves context from past conversations, decisions, and code. Use when user asks to remember something, search past conversations, recall what was done before, save context for later, or find information from previous sessions. Do NOT use for git history or file-based notes.
triggers:
  - "remember"
  - "search past"
  - "recall"
  - "what was done"
  - "previous session"
  - "save context"
  - "remember that"
  - "memory"
  - "ChromaDB"
  - "vector memory"
  - "persistent memory"
negatives:
  - "git history"
  - "file system"
  - "file notes"
  - "backup"
  - "database"
  - "memory admin (use chromadb)"
  - "backup memory (use chromadb)"
license: MIT
compatibility: opencode
metadata:
  workflow: productivity
  audience: developers
  version: "1.0.0"
  author: shokunin
allowed-tools: Read Bash Write
---


# Memory

Persistent memory across sessions using ChromaDB vector search. Every conversation is stored and retrievable.

## How It Works

The memory system uses ChromaDB (local vector database, no server needed) to store conversation context as embeddings. When you start
```

</details>
