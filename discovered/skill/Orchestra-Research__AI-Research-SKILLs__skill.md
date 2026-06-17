---
name: Orchestra-Research__AI-Research-SKILLs__skill
source: https://github.com/Orchestra-Research/AI-Research-SKILLs/blob/28f2d29236f2bade2eb92cadb2585189589a5828/15-rag/qdrant/SKILL.md
repo: Orchestra-Research/AI-Research-SKILLs
kind: skill
stars: 9694
last_pushed: 2026-04-28T05:09:27Z
license: mit
score: 9
domains: [agents-ai, vector-databases, rag, backend]
tags: [qdrant, vector-search, rag, python]
curated: 2026-06-15
curated_by: config-scout
---

# Orchestra-Research/AI-Research-SKILLs — skill

**Why it's worth keeping:** Provides high-value decision logic (when to use vs. alternatives) and complete end-to-end code workflows rather than just API snippets.

**Summary:** A comprehensive implementation guide for Qdrant that covers setup, advanced configuration (HNSW), and specific RAG integration patterns.

**Source credibility:** Highly credible; the source repository is well-starred, specialized in AI engineering, and recently updated.

**Recency:** Current; utilizes modern qdrant-client patterns suitable for contemporary agentic workflows.

**Source:** [Orchestra-Research/AI-Research-SKILLs/15-rag/qdrant/SKILL.md](https://github.com/Orchestra-Research/AI-Research-SKILLs/blob/28f2d29236f2bade2eb92cadb2585189589a5828/15-rag/qdrant/SKILL.md) · 9694★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: qdrant-vector-search
description: High-performance vector similarity search engine for RAG and semantic search. Use when building production RAG systems requiring fast nearest neighbor search, hybrid search with filtering, or scalable vector storage with Rust-powered performance.
version: 1.0.0
author: Orchestra Research
license: MIT
tags: [RAG, Vector Search, Qdrant, Semantic Search, Embeddings, Similarity Search, HNSW, Production, Distributed]
dependencies: [qdrant-client>=1.12.0]
---

# Qdrant - Vector Similarity Search Engine

High-performance vector database written in Rust for production RAG and semantic search.

## When to use Qdrant

**Use Qdrant when:**
- Building production RAG systems requiring low latency
- Need hybrid search (vectors + metadata filtering)
- Require horizontal scaling with sharding/replication
- Want on-premise deployment with full data control
- Need multi-vector storage per record (dense + sparse)
- Building real-time recommendation systems

**Key features:**
- **Rust-powered**: Memory-safe, high performance
- **Rich filtering**: Filter by any payload field during search
- **Multiple vectors**: Dense, sparse, multi-dense per point
- **Quanti
```

</details>
