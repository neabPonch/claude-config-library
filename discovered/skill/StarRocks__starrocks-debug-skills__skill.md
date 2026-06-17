---
name: StarRocks__starrocks-debug-skills__skill
source: https://github.com/StarRocks/starrocks-debug-skills/blob/6237680f6798e2d6c90b94f4b5ba15e3f469cd93/high-concurrency/SKILL.md
repo: StarRocks/starrocks-debug-skills
kind: skill
stars: 56
last_pushed: 2026-05-26T07:40:03Z
license: apache-2.0
score: 9
domains: [databases, performance-tuning, observability]
tags: [high-concurrency, starrocks, troubleshooting]
curated: 2026-06-15
curated_by: config-scout
---

# StarRocks/starrocks-debug-skills — skill

**Why it's worth keeping:** It provides specific diagnostic one-liners (shell/SQL) and maps observed metric patterns directly to root causes using an expert decision tree.

**Summary:** A specialized debugging playbook for diagnosing performance bottlenecks in high-concurrency StarRocks workloads, covering connection pooling, query cache, and pipeline parallelism.

**Source credibility:** High; official repository from the StarRocks engineering team with active maintenance.

**Recency:** Current; utilizes modern observability-driven troubleshooting workflows.

**Source:** [StarRocks/starrocks-debug-skills/high-concurrency/SKILL.md](https://github.com/StarRocks/starrocks-debug-skills/blob/6237680f6798e2d6c90b94f4b5ba15e3f469cd93/high-concurrency/SKILL.md) · 56★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: high-concurrency
description: "Use when optimizing for high-QPS (thousands of queries/sec) workloads or diagnosing throughput plateaus and latency spikes under load. Covers pipeline_dop=1 tuning, connection pooling (HikariCP/Druid), PreparedStatement plan caching, query cache hit-rate analysis, PK model point-query optimization (short-circuit scan, persistent index), and detecting session-level timeout overrides that cause memory volatility."
version: 2.0.0
category: high-concurrency
keywords:
- high QPS
- connection pool
- PreparedStatement
- query cache
- pipeline_dop
- primary key
- short circuit
tools:
- find
related_cases:
- case-015-memory-volatility
---

# High-Concurrency Best Practices

Investigation and tuning guide for high-QPS workloads: data modeling, primary-key
optimization, query cache, pipeline parallelism, connection pooling, and emergency
load disabling.

Five root causes account for most high-concurrency performance problems:

- **Cause A** — Connection pool exhausted (too many connections, no client pool)
- **Cause B** — FE planning CPU saturation (complex queries, no plan cache)
- **Cause C** — `pipeline_dop` too high for short queries (scheduling ov
```

</details>
