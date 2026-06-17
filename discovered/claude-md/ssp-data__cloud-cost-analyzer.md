---
name: ssp-data__cloud-cost-analyzer
source: https://github.com/ssp-data/cloud-cost-analyzer/blob/68bed1b890700f0875de018efd3040ab71684d18/CLAUDE.md
repo: ssp-data/cloud-cost-analyzer
kind: claude-md
stars: 29
last_pushed: 2026-02-19T15:51:19Z
license: unknown
score: 9
domains: [data-engineering, finops, etl]
tags: [etl, multi-cloud, infrastructure-as-code, data-pipeline]
curated: 2026-06-15
curated_by: config-scout
---

# ssp-data/cloud-cost-analyzer — claude-md

**Why it's worth keeping:** The file excels at documenting complex mode-switching logic, detailed command sets for every lifecycle stage, and critical implementation nuances like schema differences between cloud providers.

**Summary:** Provides a comprehensive guide to a dual-mode (Local/Cloud) data pipeline architecture using dlt, DuckDB, and Rill.

**Source credibility:** A niche but well-documented open-source FinOps project with specific toolchain expertise (dlt/Rill).

**Recency:** Very recent (4 months ago), highly relevant to modern data engineering stacks.

**Source:** [ssp-data/cloud-cost-analyzer/CLAUDE.md](https://github.com/ssp-data/cloud-cost-analyzer/blob/68bed1b890700f0875de018efd3040ab71684d18/CLAUDE.md) · 29★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Multi-cloud cost analytics platform combining AWS Cost and Usage Reports (CUR), GCP billing data, and Stripe revenue. Built with dlt for data ingestion, DuckDB/ClickHouse for storage, and Rill for visualization.

## Core Architecture

### Two Deployment Modes

**Local Development** (default):
- Data pipelines write to Parquet files in `viz_rill/data/`
- Rill dashboards query Parquet via DuckDB
- Command: `make run-all`

**Cloud Production**:
- Data pipelines write to ClickHouse Cloud
- Rill dashboards query ClickHouse directly
- Command: `make run-all-cloud`
- Requires: ClickHouse credentials in `.dlt/secrets.toml`

Mode is controlled by `DLT_DESTINATION` environment variable (set in Makefile automatically).

### Data Flow

```
1. EXTRACT (dlt incremental pipelines)
   - pipelines/aws_pipeline.py → S3 CUR Parquet
   - pipelines/google_bq_incremental_pipeline.py → BigQuery billing export
   - pipelines/stripe_pipeline.py → Stripe API

2. LOAD (write_disposition="append" for cost data, "merge" for AWS)
   - Local: → viz_rill/data/*.parquet
   - Clo
```

</details>
