---
name: dioptx__mcp-atom-of-thoughts
source: https://github.com/dioptx/mcp-atom-of-thoughts/blob/96306630e739bd453eb7257c68831059635918f0/CLAUDE.md
repo: dioptx/mcp-atom-of-thoughts
kind: claude-md
stars: 60
last_pushed: 2026-04-28T10:36:17Z
license: mit
score: 9
domains: [mcp, ai-agents, typescript]
tags: [reasoning-engine, structured-logic, mcp-server]
curated: 2026-06-16
curated_by: config-scout
---

# dioptx/mcp-atom-of-thoughts — claude-md

**Why it's worth keeping:** Contains highly specific testing conventions (naming patterns/Vitest) and strict logic constraints that are crucial for maintaining architectural integrity during AI coding sessions.

**Summary:** A high-density technical specification for a structured reasoning MCP server. It details architecture, tool schemas, data lifecycles, and developer workflows.

**Source credibility:** Niche but well-maintained repository with significant star count relative to its specialized purpose.

**Recency:** Very recent; aligns with current MCP and TypeScript ecosystem standards.

**Source:** [dioptx/mcp-atom-of-thoughts/CLAUDE.md](https://github.com/dioptx/mcp-atom-of-thoughts/blob/96306630e739bd453eb7257c68831059635918f0/CLAUDE.md) · 60★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# mcp-atom-of-thoughts (v3)

MCP server for structured reasoning via Atom of Thoughts. Decomposes problems into atomic units (premise → reasoning → hypothesis → verification → conclusion) with confidence tracking, session scoping, and on-demand D3 visualization.

## Architecture

```
index.ts          — MCP server entry, tool dispatch, viz attachment, approval server
atom-server.ts    — Full AoT (depth 5, decomposition-contraction) with session-scoped state
atom-light-server.ts — AoT-fast (depth 3) — extends atom-server, lighter response shape
tools.ts          — MCP tool definitions (3 tools)
types.ts          — AtomData, Session, GraphNode, GraphLink, ApprovalResult
config.ts         — CLI arg parsing (--mode, --viz, --max-depth, --output-dir, --downloads-dir)
visualization.ts  — D3.js interactive graph renderer (callback URL embedded)
graph-export.ts   — JSON export of atom graph
approval.ts       — File-based approval polling (fallback path)
approval-server.ts — Local 127.0.0.1 HTTP listener for browser → server callbacks
d3-bundle.ts      — D3 asset bundler
```

## MCP Tools (3)

| Tool | Purpose |
|------|---------|
| `AoT-fast` | Default reasoning. Depth 3, auto-suggests con
```

</details>
