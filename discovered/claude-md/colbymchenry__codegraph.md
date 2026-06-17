---
name: colbymchenry__codegraph
source: https://github.com/colbymchenry/codegraph/blob/2f6316500df3c8959528243aa2c837d5735d5dcd/CLAUDE.md
repo: colbymchenry/codegraph
kind: claude-md
stars: 49290
last_pushed: 2026-06-15T06:47:26Z
license: mit
score: 10
domains: [cli-tools, agents-ai, developer-tools]
tags: [architecture, mcp, tree-sitter, node-js]
curated: 2026-06-15
curated_by: config-scout
---

# colbymchenry/codegraph — claude-md

**Why it's worth keeping:** It includes critical 'tribal knowledge' like exact type string constants, Node.js version constraints, and specific tool-call optimization targets which prevent regression.

**Summary:** A highly technical guide that provides deep architectural mental models, including a layered pipeline and detailed module layout.

**Source credibility:** High; the repository is highly starred and clearly maintained by a sophisticated engineering team.

**Recency:** Very current; explicitly optimized for Claude Code and MCP workflows.

**Source:** [colbymchenry/codegraph/CLAUDE.md](https://github.com/colbymchenry/codegraph/blob/2f6316500df3c8959528243aa2c837d5735d5dcd/CLAUDE.md) · 49290★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

CodeGraph is a local-first code intelligence library + CLI + MCP server. It parses any supported codebase with tree-sitter, stores symbols/edges/files in SQLite (FTS5), and exposes a knowledge graph to AI agents (Claude Code, Cursor, Codex CLI, opencode) over MCP. Per-project data lives in `.codegraph/`. Extraction is deterministic — derived from AST, not LLM-summarized.

Distributed as `@colbymchenry/codegraph` on npm; same binary serves as installer, indexer, and MCP server.

## Build, Test, Run

```bash
npm run build           # tsc + copy schema.sql and *.wasm into dist/; chmods dist/bin/codegraph.js
npm run dev             # tsc --watch
npm run clean           # rm -rf dist

npm test                # vitest run (all)
npm run test:watch
npm run test:eval       # only __tests__/evaluation/
npm run eval            # build then run __tests__/evaluation/runner.ts via tsx

npm run cli             # build then run the local dist binary

# Single test file / pattern
npx vitest run __tests__/installer-targets.test.ts
npx vitest run __tests__/extracti
```

</details>
