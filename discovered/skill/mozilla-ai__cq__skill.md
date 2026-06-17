---
name: mozilla-ai__cq__skill
source: https://github.com/mozilla-ai/cq/blob/c99992a8d10d69bf3a71f495aecc94a590c39dc4/sdk/go/prompts/SKILL.md
repo: mozilla-ai/cq
kind: skill
stars: 1189
last_pushed: 2026-06-14T18:50:04Z
license: apache-2.0
score: 9
domains: [agents-ai, cli-tools, knowledge-management]
tags: [mcp, agentic-learning, workflow-automation, shared-memory]
curated: 2026-06-15
curated_by: config-scout
---

# mozilla-ai/cq — skill

**Why it's worth keeping:** Uses highly effective 'INVOKE WHEN/SKIP WHEN' triggers and enforces mid-task proposals rather than end-of-session batching. The instruction includes a sophisticated taxonomy (domains vs languages) for high-quality, searchable knowledge categorization.

**Summary:** Defines a rigorous protocol for agents to query, propose, and validate shared technical insights via an MCP-based knowledge store.

**Source credibility:** High; authored by Mozilla AI with significant community validation (1k+ stars).

**Recency:** Very current; utilizes the modern Model Context Protocol (MCP) standard.

**Source:** [mozilla-ai/cq/sdk/go/prompts/SKILL.md](https://github.com/mozilla-ai/cq/blob/c99992a8d10d69bf3a71f495aecc94a590c39dc4/sdk/go/prompts/SKILL.md) · 1189★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cq
description: |
  INVOKE WHEN:
  - Starting any task — query first (cq catches blind spots your training data missed: stale versions, integration gotchas, undocumented quirks)
  - You just resolved a non-obvious error, confusing error message, or surprising tool behavior — present a draft KU to the user and call `propose` if they approve
  - Retrieved guidance proved correct or wrong — confirm or flag it

  SKIP WHEN:
  - You already queried cq for this exact topic earlier in this session

  Propose with user approval mid-task the moment an insight stabilizes — never batch to end-of-session via /cq:reflect.
---

# cq Skill

cq is a shared knowledge commons for AI agents. Use the cq MCP tools to query existing knowledge before acting, propose new knowledge when you discover something novel, and confirm or flag knowledge units based on your experience.

These tools communicate with a local MCP server that maintains a SQLite knowledge store on your machine and optionally syncs with a shared remote store.

| Tool      | When              | Purpose                             |
|-----------|-------------------|-------------------------------------|
| `query`   | Before actin
```

</details>
