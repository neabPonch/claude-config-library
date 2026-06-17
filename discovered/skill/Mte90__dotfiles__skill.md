---
name: Mte90__dotfiles__skill
source: https://github.com/Mte90/dotfiles/blob/9960928265afb1a23469c1a05d3c2cd12bf2ff8c/.config/opencode/skills/llama-index/SKILL.md
repo: Mte90/dotfiles
kind: skill
stars: 47
last_pushed: 2026-06-05T12:55:38Z
license: unknown
score: 8
domains: [agents-ai, rag, python]
tags: [llama-index, llm-framework, vector-database, rag]
curated: 2026-06-15
curated_by: config-scout
---

# Mte90/dotfiles — skill

**Why it's worth keeping:** It provides high-density code patterns for critical tasks like semantic chunking and specific provider configurations (Chroma, Pinecone), reducing LLM hallucination of outdated API calls.

**Summary:** A highly structured technical reference for the LlamaIndex framework, covering RAG pipelines, data ingestion, node parsing, and vector store integrations.

**Source credibility:** The source is a curated dotfiles repository with active maintenance and moderate community interest.

**Recency:** Very current, referencing modern models (gpt-4o) and contemporary LlamaIndex patterns.

**Source:** [Mte90/dotfiles/.config/opencode/skills/llama-index/SKILL.md](https://github.com/Mte90/dotfiles/blob/9960928265afb1a23469c1a05d3c2cd12bf2ff8c/.config/opencode/skills/llama-index/SKILL.md) · 47★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: llama-index
description: Comprehensive guide for building LLM applications with LlamaIndex, including data loaders, indexes, query engines, chat engines, vector stores, retrievers, agents, evaluation, streaming, and observability.
metadata:
  author: OSS AI Skills
  version: 1.0.0
  tags:
    - llama-index
    - llm
    - rag
    - ai
    - python
    - vector-database
    - openai
    - agents
---

# LlamaIndex Development

Complete guide for building LLM applications with LlamaIndex framework.

## Overview

LlamaIndex is a data framework for LLM applications, providing tools for data ingestion, indexing, and retrieval.

**Key Characteristics:**
- RAG (Retrieval Augmented Generation) support
- Multiple data connectors (300+)
- Various index types
- Query and chat engines
- Vector store integrations
- Agent framework

## Installation

### Setup

```bash
# Basic installation
pip install llama-index

# With OpenAI
pip install llama-index-llms-openai
pip install llama-index-embeddings-openai

# With vector stores
pip install llama-index-vector-stores-chroma
pip install llama-index-vector-stores-pinecone
pip install llama-index-vector-stores-qdrant

# With evaluation
pip inst
```

</details>
