---
name: ruvnet__ruflo__skill
source: https://github.com/ruvnet/ruflo/blob/28c81c03e3e84555a9238b3217b9f586fc0c7dbc/plugins/ruflo-ruvector/skills/vector-embed/SKILL.md
repo: ruvnet/ruflo
kind: skill
stars: 59540
last_pushed: 2026-06-15T09:28:49Z
license: mit
score: 8
domains: [agents-ai, cli-tools, rag]
tags: [embeddings, vector-search, semantic-search, node-js]
curated: 2026-06-15
curated_by: config-scout
---

# ruvnet/ruflo — skill

**Why it's worth keeping:** Excellent use of 'defensive documentation' by explicitly noting missing CLI flags (--file) and prescribing how to handle them manually to prevent agent errors.

**Summary:** Provides a robust workflow for generating text embeddings using the ruvector CLI tool, including dependency management and specific command patterns.

**Source credibility:** High-star (59k+) meta-harness repository with very active maintenance.

**Recency:** Current; utilizes specific version pinning for deterministic execution in Claude Code environments.

**Source:** [ruvnet/ruflo/plugins/ruflo-ruvector/skills/vector-embed/SKILL.md](https://github.com/ruvnet/ruflo/blob/28c81c03e3e84555a9238b3217b9f586fc0c7dbc/plugins/ruflo-ruvector/skills/vector-embed/SKILL.md) · 59540★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: vector-embed
description: Generate embeddings via npx ruvector@0.2.25 embed text (ONNX all-MiniLM-L6-v2, 384-dim), normalize, and store in HNSW index
argument-hint: "<text-or-file>"
allowed-tools: Bash Read mcp__claude-flow__memory_store mcp__claude-flow__memory_search
---

# Vector Embed

Generate and store vector embeddings using the `ruvector` npm package.

## When to use

Use this skill to embed text, code, or documents into 384-dimensional vectors for semantic search, similarity comparison, or clustering. ruvector uses ONNX all-MiniLM-L6-v2 with HNSW indexing (52,000+ inserts/sec, ~0.045ms search).

## Steps

1. **Ensure ruvector@0.2.25 is available**:
   ```bash
   npm ls ruvector 2>/dev/null | grep '0.2.25' || npm install ruvector@0.2.25
   ```
   If `embed text` later reports `ONNX WASM files not bundled`, also run:
   ```bash
   npm install ruvector-onnx-embeddings-wasm
   ```
2. **Embed the input** (use the `text` subcommand, with text as a positional arg):
   - Single string: `npx -y ruvector@0.2.25 embed text "your text here"`
   - With output file: `npx -y ruvector@0.2.25 embed text "your text here" -o vec.json`
   - For a file: read its content via the Read
```

</details>
