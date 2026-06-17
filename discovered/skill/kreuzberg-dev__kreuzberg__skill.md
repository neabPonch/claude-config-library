---
name: kreuzberg-dev__kreuzberg__skill
source: https://github.com/kreuzberg-dev/kreuzberg/blob/f5d6107cb14bd1a3b3db5d1ac681081c85eae5d3/.ai-rulez/skills/chunking-embeddings/SKILL.md
repo: kreuzberg-dev/kreuzberg
kind: skill
stars: 8490
last_pushed: 2026-06-15T04:30:32Z
license: other
score: 8
domains: [agents-ai, data-engineering]
tags: [rag, chunking, embeddings, document-intelligence]
curated: 2026-06-15
curated_by: config-scout
---

# kreuzberg-dev/kreuzberg — skill

**Why it's worth keeping:** The 'Critical Rules' section provides highly actionable engineering heuristics (e.g., overlap percentages and batching requirements) that are easily transferable to other agentic workflows.

**Summary:** Defines a rigorous technical pipeline for document chunking, embedding generation, and RAG integration using the Kreuzberg framework.

**Source credibility:** High; source repository has strong social proof with 8k+ stars and recent maintenance.

**Recency:** Current; aligns perfectly with modern RAG and document intelligence best practices.

**Source:** [kreuzberg-dev/kreuzberg/.ai-rulez/skills/chunking-embeddings/SKILL.md](https://github.com/kreuzberg-dev/kreuzberg/blob/f5d6107cb14bd1a3b3db5d1ac681081c85eae5d3/.ai-rulez/skills/chunking-embeddings/SKILL.md) · 8490★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
description: "Chunking, embeddings, and RAG pipeline integration"
name: chunking-embeddings
priority: critical
---

# Chunking & Embeddings

**Text splitting strategies, embedding generation with FastEmbed, RAG pipeline integration**

## Chunking Architecture Overview

**Location**: `crates/kreuzberg/src/chunking/`, `crates/kreuzberg/src/embeddings.rs`

```text
Extracted Text
    |
[1. Normalization] -> Clean whitespace, remove control chars
    |
[2. Chunk Strategy Selection] -> Fixed-size, semantic, syntax-aware, recursive
    |
[3. Overlap Management] -> Control context window overlap
    |
[4. Optional Embedding] -> Generate vectors with FastEmbed
    |
Output: Vec<Chunk> with text, vectors, metadata
```

## Chunking Strategies

**Location**: `crates/kreuzberg/src/chunking/mod.rs`

| Strategy                          | Pattern                                                 | Best For                                                           |
| --------------------------------- | ------------------------------------------------------- | ------------------------------------------------------------------ |
| **Fixed-Size**                    | Sliding window with configurabl
```

</details>
