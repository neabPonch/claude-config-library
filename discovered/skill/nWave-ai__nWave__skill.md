---
name: nWave-ai__nWave__skill
source: https://github.com/nWave-ai/nWave/blob/23d5ccedd6f71af5a9e5ac586224559ea1b875fd/plugins/nw/skills/nw-data-architecture-patterns/SKILL.md
repo: nWave-ai/nWave
kind: skill
stars: 544
last_pushed: 2026-06-15T11:22:54Z
license: other
score: 8
domains: [data-engineering, architecture]
tags: [data-warehouse, etl-elt, scaling]
curated: 2026-06-15
curated_by: config-scout
---

# nWave-ai/nWave — skill

**Why it's worth keeping:** It uses structured decision trees and 'Use when/Avoid when' frameworks that allow an agent to act as a senior architect. The inclusion of specific anti-patterns and scaling strategies provides actionable guidance rather than just definitions.

**Summary:** Provides a high-density knowledge base of data architecture patterns including warehouse, lakehouse, and mesh structures.

**Source credibility:** nWave-ai is a specialized AI agent repo with significant social proof (544 stars).

**Recency:** Very current, featuring modern standards like Medallion architecture and Apache Iceberg.

**Source:** [nWave-ai/nWave/plugins/nw/skills/nw-data-architecture-patterns/SKILL.md](https://github.com/nWave-ai/nWave/blob/23d5ccedd6f71af5a9e5ac586224559ea1b875fd/plugins/nw/skills/nw-data-architecture-patterns/SKILL.md) · 544★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: nw-data-architecture-patterns
description: Data architecture patterns (warehouse, lake, lakehouse, mesh), ETL/ELT pipelines, streaming architectures, scaling strategies, and schema design patterns
user-invocable: false
disable-model-invocation: true
---

# Data Architecture Patterns

## Architecture Selection Decision Tree

Structured only -> **Data Warehouse** | Mixed + SQL analytics -> **Data Lakehouse** | Mixed + ML-primary -> **Data Lake** | Large org + autonomous domains -> **Data Mesh**

## Data Warehouse

Schema: structured, schema-on-write | Data: tables, rows, columns | Governance: centralized | Query: SQL analytics, BI | Architecture: centralized single source of truth

### Schema Patterns

**Star Schema**: Central fact table (measures) surrounded by denormalized dimension tables. Best for BI dashboards, standard reporting.

**Snowflake Schema**: Normalized dimensions (dimensions reference other dimensions). Reduces storage, increases JOIN complexity. Best when storage cost matters more than query speed.

### Kimball vs Inmon

**Kimball (Bottom-Up)**: Build data marts first, integrate later | Star schema, business-process driven | Faster initial delivery | Best
```

</details>
