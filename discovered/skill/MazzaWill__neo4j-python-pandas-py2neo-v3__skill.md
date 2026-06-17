---
name: MazzaWill__neo4j-python-pandas-py2neo-v3__skill
source: https://github.com/MazzaWill/neo4j-python-pandas-py2neo-v3/blob/2e2b08d36e8c23132d1f0822f155426145789d7e/skills/neo4j-knowledge-graph/SKILL.md
repo: MazzaWill/neo4j-python-pandas-py2neo-v3
kind: skill
stars: 579
last_pushed: 2026-06-12T18:40:03Z
license: mit
score: 9
domains: [data-engineering, knowledge-graphs, ai-agents]
tags: [neo4j, graphrag, cypher, data-modeling]
curated: 2026-06-16
curated_by: config-scout
---

# MazzaWill/neo4j-python-pandas-py2neo-v3 — skill

**Why it's worth keeping:** It enforces expert engineering patterns like profiling raw data before modeling, using MERGE/UNWIND for imports, and establishing uniqueness constraints to prevent graph corruption.

**Summary:** Provides a rigorous workflow for transforming tabular data into Neo4j knowledge graphs, covering modeling, safe Cypher generation, and GraphRAG integration.

**Source credibility:** High; the repository has significant community traction (579 stars) and active maintenance.

**Recency:** Current; incorporates modern Neo4j 5+ practices, official drivers, and GraphRAG/vector search workflows.

**Source:** [MazzaWill/neo4j-python-pandas-py2neo-v3/skills/neo4j-knowledge-graph/SKILL.md](https://github.com/MazzaWill/neo4j-python-pandas-py2neo-v3/blob/2e2b08d36e8c23132d1f0822f155426145789d7e/skills/neo4j-knowledge-graph/SKILL.md) · 579★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: neo4j-knowledge-graph
description: Use when designing, importing, querying, or modernizing Neo4j knowledge graphs from CSV, Excel, pandas, Cypher, py2neo, the official neo4j Python driver, vector indexes, or GraphRAG workflows.
---

# Neo4j Knowledge Graph

## Overview

Use this skill to turn tabular or semi-structured data into a Neo4j knowledge graph, then choose the right path: legacy py2neo compatibility, modern official-driver Cypher, or GraphRAG/vector search.

## Workflow

1. **Frame the graph task**
   - Identify the source data: CSV, Excel, pandas DataFrame, database export, API data, or existing Neo4j graph.
   - Ask what the user wants to do: import, model, query, migrate, visualize, or add GraphRAG.
   - Confirm Neo4j target: local Neo4j, Aura, legacy Neo4j 3.x, Neo4j 5+, or unknown.

2. **Profile data before modeling**
   - For CSV/Excel files, run `scripts/profile_table.py <path>` when local files are available.
   - Inspect columns, sample values, blank counts, likely identifiers, and repeated values.
   - Do not infer graph labels from one row only.

3. **Model the graph**
   - Use nouns for labels: `Invoice`, `Person`, `Company`, `Product`, `Location`.
```

</details>
