---
name: newgnart__token-transfer-analytics
source: https://github.com/newgnart/token-transfer-analytics/blob/9d5986ab8c57a6308e786cbdd8db7d337fb0e3e7/CLAUDE.md
repo: newgnart/token-transfer-analytics
kind: claude-md
stars: 1
last_pushed: 2026-01-24T03:39:57Z
license: unknown
score: 9
domains: [data-engineering, etl-pipeline]
tags: [dbt, airflow, python, architecture-map]
curated: 2026-06-15
curated_by: config-scout
---

# newgnart/token-transfer-analytics — claude-md

**Why it's worth keeping:** It provides a clear visual architecture diagram and high-density command patterns (using `uv`) that allow Claude to execute complex tasks without ambiguity.

**Summary:** A comprehensive technical manual for an ELT data pipeline involving Airflow, dbt, and Snowflake/PostgreSQL. It maps the entire lifecycle from raw extraction to final analytics tables.

**Source credibility:** High-quality capstone project with professional-grade documentation structure.

**Recency:** Recent (5 months ago) and utilizes modern tooling like `uv` and dbt.

**Source:** [newgnart/token-transfer-analytics/CLAUDE.md](https://github.com/newgnart/token-transfer-analytics/blob/9d5986ab8c57a6308e786cbdd8db7d337fb0e3e7/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Stables Analytics is a capstone project for Foundry AI Academy (DAE2) - a production-grade ELT pipeline for on-chain stablecoin analytics. The project extracts blockchain data via HyperSync GraphQL API, loads it into PostgreSQL/Snowflake, and transforms it using dbt.

## Architecture

**Pipeline**: `HyperSync GraphQL → Kafka → PostgreSQL/Snowflake → dbt → Analytics Tables`

The project follows an event-driven ELT (Extract, Load, Transform) pattern with Kafka streaming and Airflow orchestration:

```
┌─────────────────────────────────────────────────────────────────┐
│                   Apache Airflow (Orchestration)                 │
└─────────────────────────────────────────────────────────────────┘
         │                    │                      │
         ▼                    ▼                      ▼
  Kafka Monitoring      Consumer Control       dbt Transform
  (Health/Lag)          (Load to DB)          (Analytics)
         │                    │                      │
         ▼                    ▼                      ▼
  GraphQL → K
```

</details>
