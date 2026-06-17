---
name: osodevops__k2i
source: https://github.com/osodevops/k2i/blob/f85d3e74a9cdda44847b2e874928e4d9a15f4042/claude.md
repo: osodevops/k2i
kind: claude-md
stars: 20
last_pushed: 2026-05-05T11:18:30Z
license: other
score: 9
domains: [systems-programming, data-engineering, rust]
tags: [architecture-heavy, state-management, performance-critical]
curated: 2026-06-15
curated_by: config-scout
---

# osodevops/k2i — claude-md

**Why it's worth keeping:** The 'Key Design Decisions' and 'Crash Recovery Guarantees' sections provide the AI with critical logic boundaries to prevent incorrect refactoring of state management or error handling.

**Summary:** Provides deep architectural context, data flow diagrams, and specific design constraints for a high-performance Rust streaming engine.

**Source credibility:** High-quality technical documentation reflecting a sophisticated, specialized engineering tool.

**Recency:** Very current; uses modern Rust (1.85+) and contemporary library versions.

**Source:** [osodevops/k2i/claude.md](https://github.com/osodevops/k2i/blob/f85d3e74a9cdda44847b2e874928e4d9a15f4042/claude.md) · 20★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# K2I - Kafka to Iceberg Streaming Ingestion Engine

## What This Project Is

K2I is a production-grade streaming ingestion engine written in Rust that bridges the latency-cost gap in modern data pipelines. It consumes events from Apache Kafka, buffers them in-memory using Apache Arrow for sub-second query freshness, and writes them to Apache Iceberg tables in Parquet format with exactly-once semantics.

## Why We Built It

The data engineering world forces a painful trade-off:
- **Real-time systems** (Flink, KSQL): millisecond latency but high cost and operational complexity
- **Batch systems** (Spark, Airflow): low cost but minutes-to-hours of latency

K2I delivers **sub-second data freshness at batch economics** through a single-process architecture that eliminates distributed coordination overhead. It is inspired by Moonlink (pg_mooncake) but purpose-built for Kafka-native workloads rather than CDC.

## Core Concepts

### Hot/Cold Data Separation
- **Hot buffer**: In-memory Arrow RecordBatches with DashMap indexes for <1ms query lookups
- **Cold storage**: Parquet files on object storage (S3/GCS/Azure) committed to Iceberg catalogs

### Single-Process Simplicity
No cluster coor
```

</details>
