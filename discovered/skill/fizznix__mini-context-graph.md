---
name: fizznix__mini-context-graph
source: https://github.com/fizznix/mini-context-graph/blob/006462018a817d2eb1cbe0e21abc320430746906/skill.md
repo: fizznix/mini-context-graph
kind: skill
stars: 1
last_pushed: 2026-04-10T19:29:25Z
license: mit
score: 8
domains: [agents-ai, knowledge-management]
tags: [memory-graph, rag, long-term-context, knowledge-synthesis]
curated: 2026-06-14
curated_by: config-scout
---

# fizznix/mini-context-graph — skill

**Why it's worth keeping:** The 'Wiki-first' retrieval strategy paired with strict extraction constraints is highly effective. The specific workflows for updating entity pages during ingestion provide a clear template for building long-term agentic memory.

**Summary:** A multi-layered memory system that combines a markdown wiki for synthesis, a knowledge graph for relationships, and raw storage for provenance. It shifts the paradigm from repetitive RAG to compounding, synthesized knowledge.

**Source credibility:** Niche/low star count, but demonstrates high-level architectural sophistication and practical pattern application.

**Recency:** Current; aligns with modern trends in agentic long-term memory and structured RAG.

**Source:** [fizznix/mini-context-graph/skill.md](https://github.com/fizznix/mini-context-graph/blob/006462018a817d2eb1cbe0e21abc320430746906/skill.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: mini-context-graph
description: |
  A persistent, compounding knowledge base combining Karpathy's LLM Wiki pattern
  with a structured knowledge graph. Ingest documents once — the LLM writes wiki
  pages, extracts entities/relations into the graph, and stores raw content for
  evidence retrieval. Knowledge accumulates and cross-references; it is never
  re-derived from scratch.
---

# Mini Context Graph Skill

## The Core Idea

Standard RAG re-discovers knowledge from scratch on every query. This skill is different:

1. **Wiki layer** — The LLM writes and maintains persistent markdown pages (summaries, entity pages, topic syntheses). Cross-references are already there. The wiki gets richer with every ingest.
2. **Graph layer** — Entities and relations are extracted once and stored as a navigable knowledge graph. BFS traversal answers structural queries without re-reading sources.
3. **Raw source layer** — Original documents are stored immutably with chunks. Provenance links tie every graph node and edge back to the exact text that supports it.

> The LLM writes; the Python tools handle all bookkeeping.

---

## Three Layers

| Layer | Where | What the LLM does | What Pyth
```

</details>
