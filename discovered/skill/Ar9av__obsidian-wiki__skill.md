---
name: Ar9av__obsidian-wiki__skill
source: https://github.com/Ar9av/obsidian-wiki/blob/cc1f83f761dfae8e1324e48546e290082de97d80/.skills/wiki-agent/SKILL.md
repo: Ar9av/obsidian-wiki
kind: skill
stars: 2024
last_pushed: 2026-06-14T07:37:53Z
license: mit
score: 9
domains: [agents-ai, knowledge-management, cli-tools, automation]
tags: [ingestion, context-retrieval, multi-agent]
curated: 2026-06-15
curated_by: config-scout
---

# Ar9av/obsidian-wiki — skill

**Why it's worth keeping:** Uses 'cheapest index source' logic to avoid heavy I/O and implements a multi-factor scoring algorithm (title, CWD, recency) for high-precision extraction.

**Summary:** Provides a highly sophisticated pattern for query-driven context retrieval across multiple distinct AI agent histories and into an Obsidian wiki.

**Source credibility:** Strong; follows a proven architectural pattern with active recent maintenance and significant community interest.

**Recency:** Very current; specifically maps the file structures of modern CLI-based AI agents.

**Source:** [Ar9av/obsidian-wiki/.skills/wiki-agent/SKILL.md](https://github.com/Ar9av/obsidian-wiki/blob/cc1f83f761dfae8e1324e48546e290082de97d80/.skills/wiki-agent/SKILL.md) · 2024★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: wiki-agent
description: >
  Query-driven targeted ingest from a specific AI agent's raw history. Use this skill when the user
  invokes /wiki-claude, /wiki-codex, /wiki-hermes, /wiki-openclaw, /wiki-copilot, /wiki-pi — with or without a
  search topic. Different from wiki-history-ingest (which bulk-ingests everything new): this skill finds
  sessions about a SPECIFIC TOPIC in a specific agent's history and ingests just those, then returns a
  synthesized answer immediately usable in the current session. Primary use case: you're working in
  agent A and want to pull in how you solved X in agent B's history. Cross-referencing, not archiving.
  Also trigger on: "what did I work on in codex about X", "search my claude sessions for Y",
  "pull in hermes knowledge about Z", "find that conversation where I did X in codex".
---

# Wiki Agent — Targeted Cross-Agent History Search + Ingest

You are doing a **query-driven targeted ingest** from one specific AI agent's raw conversation history. The user is typically working in a *different* agent right now and wants to pull in context from another agent's past sessions.

This is not bulk ingest. You find sessions about a specific top
```

</details>
