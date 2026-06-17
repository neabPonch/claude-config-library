---
name: wshobson__agents__skill
source: https://github.com/wshobson/agents/blob/cc37bfdd292ce520ba1c44df7a3a70d5f8137236/plugins/data-engineering/skills/spark-optimization/SKILL.md
repo: wshobson/agents
kind: skill
stars: 36755
last_pushed: 2026-06-15T01:09:29Z
license: mit
score: 8
domains: [data-engineering, big-data]
tags: [optimization, spark, performance]
curated: 2026-06-15
curated_by: config-scout
---

# wshobson/agents — skill

**Why it's worth keeping:** Includes high-density technical constants (AQE/Kryo settings) and a comparative table of performance bottlenecks that provide excellent context for an agent's reasoning.

**Summary:** Provides a structured domain-knowledge framework for optimizing Apache Spark jobs through execution models and configuration patterns.

**Source credibility:** High; the source repository is highly starred and actively maintained.

**Recency:** Current; uses modern Spark optimization techniques like Adaptive Query Execution (AQE).

**Source:** [wshobson/agents/plugins/data-engineering/skills/spark-optimization/SKILL.md](https://github.com/wshobson/agents/blob/cc37bfdd292ce520ba1c44df7a3a70d5f8137236/plugins/data-engineering/skills/spark-optimization/SKILL.md) · 36755★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: spark-optimization
description: Optimize Apache Spark jobs with partitioning, caching, shuffle optimization, and memory tuning. Use when improving Spark performance, debugging slow jobs, or scaling data processing pipelines.
---

# Apache Spark Optimization

Production patterns for optimizing Apache Spark jobs including partitioning strategies, memory management, shuffle optimization, and performance tuning.

## When to Use This Skill

- Optimizing slow Spark jobs
- Tuning memory and executor configuration
- Implementing efficient partitioning strategies
- Debugging Spark performance issues
- Scaling Spark pipelines for large datasets
- Reducing shuffle and data skew

## Core Concepts

### 1. Spark Execution Model

```
Driver Program
    ↓
Job (triggered by action)
    ↓
Stages (separated by shuffles)
    ↓
Tasks (one per partition)
```

### 2. Key Performance Factors

| Factor            | Impact                | Solution                      |
| ----------------- | --------------------- | ----------------------------- |
| **Shuffle**       | Network I/O, disk I/O | Minimize wide transformations |
| **Data Skew**     | Uneven task duration  | Salting, broadcast joins
```

</details>
