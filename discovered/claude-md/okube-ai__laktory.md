---
name: okube-ai__laktory
source: https://github.com/okube-ai/laktory/blob/27040080ac1da2e3705c923ae25ee6feb393e4f4/CLAUDE.md
repo: okube-ai/laktory
kind: claude-md
stars: 57
last_pushed: 2026-06-05T17:23:30Z
license: mit
score: 9
domains: [data-engineering, cli-tools, devops]
tags: [structured-docs, multi-repo-rules, directory-mapping]
curated: 2026-06-16
curated_by: config-scout
---

# okube-ai/laktory — claude-md

**Why it's worth keeping:** Demonstrates advanced patterns for cross-repo permission boundaries and uses a 'documentation map' to link specific topics to deep-dive files.

**Summary:** A highly structured technical guide that maps directory purposes, specific build/test commands, and deep architectural documentation via lookup tables.

**Source credibility:** High; comes from an active, specialized DataOps project with clear technical depth.

**Recency:** Highly current, utilizing modern tooling like uv and structured for Claude Code's context requirements.

**Source:** [okube-ai/laktory/CLAUDE.md](https://github.com/okube-ai/laktory/blob/27040080ac1da2e3705c923ae25ee6feb393e4f4/CLAUDE.md) · 57★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Laktory

## Project Overview

Laktory is a DataOps and ETL framework for building lakehouses on Databricks. It combines:
- **Data pipeline definitions** as code (transformations, sources, sinks)
- **Infrastructure-as-Code** for Databricks resources (Unity Catalog, compute, access grants)
- **Multi-backend dataframe support** via Narwhals (Spark and Polars)
- **Multiple orchestrator support** (local, Databricks Jobs/Declarative Pipelines, Apache Airflow)

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Language | Python 3.10+ |
| Data modeling | Pydantic v2 |
| DataFrame abstraction | Narwhals |
| DataFrame backends | Apache Spark (PySpark), Polars |
| SQL parsing | SQLGlot |
| IaC backends | Pulumi, Terraform |
| CLI | Typer |
| DAG management | NetworkX |

## Key Directories

| Path | Purpose |
|------|---------|
| `laktory/models/` | All Pydantic models - the core of the library |
| `laktory/models/resources/databricks/` | 50+ Databricks resource definitions (Catalog, Job, Cluster, etc.) |
| `laktory/models/pipeline/` | Pipeline, PipelineNode, and execution plan |
| `laktory/models/datasources/` | Input sources (file, Unity Catalog, Hive, DataFrame, node) |
| `lak
```

</details>
