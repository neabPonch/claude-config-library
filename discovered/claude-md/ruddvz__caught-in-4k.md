---
name: ruddvz__caught-in-4k
source: https://github.com/ruddvz/caught-in-4k/blob/c29323a4e20b109653fa5a13c70f7b88432e740a/claude.md
repo: ruddvz/caught-in-4k
kind: claude-md
stars: 1
last_pushed: 2026-06-14T15:10:07Z
license: other
score: 9
domains: [agents-ai, cli-tools, context-management]
tags: [token-efficiency, codemaps, agent-orchestration]
curated: 2026-06-14
curated_by: config-scout
---

# ruddvz/caught-in-4k — claude-md

**Why it's worth keeping:** The 'RTK' prefix pattern for minimizing output tokens and the 'Codemap' strategy for targeted file navigation are elite context management techniques.

**Summary:** Implements a multi-agent ecosystem and unique token-saving protocols through command prefixing and hierarchical documentation.

**Source credibility:** Low star count, but highly technical and specific content suggests a high-effort, custom configuration.

**Recency:** 

**Source:** [ruddvz/caught-in-4k/claude.md](https://github.com/ruddvz/caught-in-4k/blob/c29323a4e20b109653fa5a13c70f7b88432e740a/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

**Caught in 4K (C4K)** — Gen Z-themed, AI-powered streaming platform. Streams movies and shows with AI-generated "Canon Takes" (Pollinations primary, Gemini fallback).

## Token Efficiency — MANDATORY

This project uses three token-saving stacks. All agents MUST use them:

1. **RTK** — Prefix ALL shell commands with `rtk`. Saves 60-90% tokens on command output.
   ```bash
   rtk git status          # not: git status
   rtk npm run build       # not: npm run build
   rtk npm test            # not: npm test
   rtk git diff -- file.js # not: git diff (entire repo)
   ```

2. **CODEMAPS** — Never scan the full codebase. Read `docs/CODEMAPS/OVERVIEW.md` first, drill into the specific codemap, then read only the files you'll modify.

3. **Memstack** — Check Claude memory for past decisions before re-learning. Don't repeat what's already known.

## Agent Ecosystem

This project uses the **C4K Agent Ecosystem** — 4 specialized agents that communicate via structured contracts. See `docs/superpowers/specs/c4k-agent-ecosystem.md` for the full spec.

| Agent | Role | Files |
|-------|------|-------|
| **C4K Orchestrator** | Dispatch, coordination, completion t
```

</details>
