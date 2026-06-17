---
name: teman67__AI-Powered-Material-Science-Knowledge-Graph-Platform
source: https://github.com/teman67/AI-Powered-Material-Science-Knowledge-Graph-Platform/blob/d950a0bea6c47c3ef4004b822a1622d8201755fe/Claude.md
repo: teman67/AI-Powered-Material-Science-Knowledge-Graph-Platform
kind: claude-md
stars: 1
last_pushed: 2026-05-11T11:02:45Z
license: unknown
score: 8
domains: [ai-agents, knowledge-graphs, rag-pipeline, data-engineering]
tags: [scientific-ai, rdf, graph-rag, full-stack]
curated: 2026-06-14
curated_by: config-scout
---

# teman67/AI-Powered-Material-Science-Knowledge-Graph-Platform — claude-md

**Why it's worth keeping:** It provides high-density context including explicit database schemas (SQL/RDF), specific data transformation pipelines, and clear service boundaries that prevent agent hallucination.

**Summary:** A comprehensive technical specification and implementation blueprint for a complex scientific RAG system using Knowledge Graphs and RDF.

**Source credibility:** Low social proof (1 star) but contains highly detailed, domain-specific technical architecture.

**Recency:** Very current, utilizing modern stacks like Python 3.12 and sophisticated GraphRAG patterns.

**Source:** [teman67/AI-Powered-Material-Science-Knowledge-Graph-Platform/Claude.md](https://github.com/teman67/AI-Powered-Material-Science-Knowledge-Graph-Platform/blob/d950a0bea6c47c3ef4004b822a1622d8201755fe/Claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AI-Powered Material Science Knowledge Graph Platform

## Full Implementation Guide for AI Coding Agents

---

# 1. Project Overview

## Goal

Build a full-stack AI platform that:

1. Accepts material science papers (PDFs)
2. Extracts scientific knowledge
3. Maps extracted information to the PMDcore ontology
4. Generates RDF triples
5. Stores data in a Knowledge Graph
6. Performs semantic search using RAG
7. Answers scientific questions using LLMs
8. Visualizes relationships between materials, properties, and processes

---

# 2. Main Features

## Core Features

- PDF Upload
- Scientific Text Extraction
- Chunking Pipeline
- Embedding Generation
- Vector Search
- LLM-based Question Answering
- Ontology-aware Entity Extraction
- RDF Triple Generation
- SHACL Validation
- Knowledge Graph Visualization
- Authentication
- Async Processing
- API Endpoints
- Graph-based Retrieval

---

# 3. Target Architecture

```text
Frontend (Next.js)
        |
        v
FastAPI Backend
        |
        +----------------------+
        |                      |
        v                      v
PostgreSQL + pgvector     Neo4j / GraphDB
        |                      |
        v                      v
```

</details>
