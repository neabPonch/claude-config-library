---
name: 1517005260__graph-rag-agent
source: https://github.com/1517005260/graph-rag-agent/blob/4296b7c66307a856d0467c6ca635534c447c976b/CLAUDE.md
repo: 1517005260/graph-rag-agent
kind: claude-md
stars: 2226
last_pushed: 2025-11-05T08:15:51Z
license: mit
score: 9
domains: [agents-ai, knowledge-graphs, backend-api]
tags: [rag, multi-agent, graph-database, llm-orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# 1517005260/graph-rag-agent — claude-md

**Why it's worth keeping:** Includes a critical 'Known Issues & Compatibility' section that prevents the AI from suggesting incompatible models or hitting known timeouts. Its detailed command registry makes it highly actionable for automated task execution.

**Summary:** Comprehensive guide covering complex architecture, three-tier configuration hierarchies, and specific execution pipelines.

**Source credibility:** High; the repository has significant community traction (2k+ stars) and specific technical depth.

**Recency:** Very recent; includes compatibility notes for modern models like DeepSeek-V3/R1 era releases.

**Source:** [1517005260/graph-rag-agent/CLAUDE.md](https://github.com/1517005260/graph-rag-agent/blob/4296b7c66307a856d0467c6ca635534c447c976b/CLAUDE.md) · 2226★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a GraphRAG + Deep Search implementation with multi-agent collaboration system. The project combines knowledge graph construction, entity disambiguation, community detection, and multiple agent types (NaiveRAG, GraphAgent, HybridAgent, DeepResearchAgent, FusionGraphRAGAgent) to build an explainable and reasoning-capable Q&A system.

**Language**: Primarily Chinese (comments, docs, UI) with English code structures.

## Architecture

### Core Package Structure (`graphrag_agent/`)

- **agents/**: Agent implementations with Plan-Execute-Report multi-agent orchestration
  - `base.py`: BaseAgent with LangGraph integration, cache managers, and stream/non-stream support
  - Individual agents: `naive_rag_agent.py`, `graph_agent.py`, `hybrid_agent.py`, `deep_research_agent.py`, `fusion_agent.py`
  - `multi_agent/`: Plan-Execute-Report architecture
    - `planner/`: Clarifier, TaskDecomposer, PlanReviewer → generates `PlanSpec`
    - `executor/`: RetrievalExecutor, ResearchExecutor, ReflectionExecutor
    - `reporter/`: OutlineBuilder, SectionWriter,
```

</details>
