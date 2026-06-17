---
name: LainePearce__card-oracle-max
source: https://github.com/LainePearce/card-oracle-max/blob/9096f963aa0839c2903ed89f032809be4cb4ebb8/Claude.md
repo: LainePearce/card-oracle-max
kind: claude-md
stars: 0
last_pushed: 2026-06-15T23:18:32Z
license: unknown
score: 9
domains: [infrastructure, data-engineering]
tags: [migration, stage-based-development, context-steering, scope-management]
curated: 2026-06-16
curated_by: config-scout
---

# LainePearce/card-oracle-max — claude-md

**Why it's worth keeping:** Uses strict stage-based guardrails (Stage 1 vs. Stage 2) and explicit 'In/Out of Scope' definitions to prevent the agent from attempting future-phase work prematurely. The directory tree uses status markers to steer navigation.

**Summary:** A high-fidelity development context file designed to guide an AI through a complex, multi-phase infrastructure migration.

**Source credibility:** Highly professional; reads like a genuine engineering design specification (SAD/EXP).

**Recency:** Current; utilizes forward-looking dates and modern vector database patterns (Qdrant).

**Source:** [LainePearce/card-oracle-max/Claude.md](https://github.com/LainePearce/card-oracle-max/blob/9096f963aa0839c2903ed89f032809be4cb4ebb8/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Card Search Platform — Vector Search Migration
## Claude Code Development Context

> **Document Reference:** DEV-VSM-2026-001  
> **Related Documents:** SAD-VSA-2026-001 (System Analysis & Design), EXP-VSC-2026-001 (Experimental Analysis)  
> **Last Updated:** March 2026  
> **Revision:** 1.5 — S3 vector store defined as primary durable store; naming convention and repopulation pipeline documented  
> **Status:** Active Development

---

## 1. Project Overview

This codebase implements the migration of the trading card search platform's vector search infrastructure from **Amazon OpenSearch Service KNN** to **Qdrant ANN**, as specified in SAD-VSA-2026-001. The project follows a **two-stage development process**. Stage 2 only begins if Stage 1 produces a successful experimental outcome.

---

### Stage 1 — Qdrant Comparative Analysis ← **CURRENT STAGE**

**Objective:** Populate a Qdrant database from the extant read-only OpenSearch cluster and run a direct comparative analysis of vector search capabilities between the two systems.

**In scope:**
- Stand up Qdrant (local dev → production cluster)
- Scroll the extant OpenSearch cluster to read all documents and generate embeddings
-
```

</details>
