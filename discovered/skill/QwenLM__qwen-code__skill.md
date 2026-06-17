---
name: QwenLM__qwen-code__skill
source: https://github.com/QwenLM/qwen-code/blob/02bd82abfd0d95a21137ab053c3eb32494ff2752/.qwen/skills/codegraph/SKILL.md
repo: QwenLM/qwen-code
kind: skill
stars: 25216
last_pushed: 2026-06-15T05:49:40Z
license: apache-2.0
score: 9
domains: [cli-tools, ai-agents, software-engineering]
tags: [knowledge-graph, code-analysis, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# QwenLM/qwen-code — skill

**Why it's worth keeping:** The transition from simple RAG/grep to a structural Knowledge Graph is a high-tier technique for managing large-scale codebase context, making it highly transferable for building advanced coding agents.

**Summary:** This tool implements a dual-layer knowledge graph (structure + evolution) to enable deep architectural analysis and impact tracing via Cypher queries. It allows an agent to move beyond file-based searching to relationship-based reasoning.

**Source credibility:** High; comes from the QwenLM ecosystem with massive community interest and regular updates.

**Recency:** Highly current, leveraging modern graph-based RAG techniques essential for agentic workflows.

**Source:** [QwenLM/qwen-code/.qwen/skills/codegraph/SKILL.md](https://github.com/QwenLM/qwen-code/blob/02bd82abfd0d95a21137ab053c3eb32494ff2752/.qwen/skills/codegraph/SKILL.md) · 25216★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: codegraph
description: Analyze indexed codebases via graph database (neug) and vector index (zvec). Covers call graphs, dependencies, dead code, hotspots, module coupling, architecture reports, semantic search, impact analysis, bug root cause from GitHub issues, class diagrams (UML), and PR review (risk scoring, conflict detection, auto-merge candidates, labeling). Also covers creating, inspecting, and repairing a CodeScope index. Use for: code structure, who calls what, why something changed, similar functions, module boundaries, bug tracing, class relationships, PR risk/conflicts, or any question benefiting from a code knowledge graph. Applies when a `.codegraph` index exists in the workspace, or when the user wants to create one.
---

# CodeScope Q&A

CodeScope indexes source code into a two-layer knowledge graph — **structure** (functions, calls, imports, classes, modules) and **evolution** (commits, file changes, function modifications) — plus **semantic embeddings** for every function. Supports **Python, JavaScript/TypeScript, C, and Java** (including Hadoop-scale repositories with 8K+ files). This combination enables analyses that grep, LSP, or pure vector search c
```

</details>
