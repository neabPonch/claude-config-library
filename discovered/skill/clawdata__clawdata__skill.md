---
name: clawdata__clawdata__skill
source: https://github.com/clawdata/clawdata/blob/f17377eaee1454a2d7a25b6e85d2b5de8dadf82d/skills/spark/SKILL.md
repo: clawdata/clawdata
kind: skill
stars: 25
last_pushed: 2026-03-08T22:38:51Z
license: unknown
score: 8
domains: [data-engineering, big-data, etl]
tags: [pyspark, apache-spark, delta-lake]
curated: 2026-06-16
curated_by: config-scout
---

# clawdata/clawdata — skill

**Why it's worth keeping:** Includes actionable spark-submit templates and high-value code snippets for common tasks like window functions and Delta merges.

**Summary:** Provides comprehensive CLI commands and PySpark patterns for data processing, including Delta Lake integration.

**Source credibility:** Niche repository focused on data engineering tools with moderate recent activity.

**Recency:** Current; includes modern best practices like Adaptive Query Execution and Delta Lake patterns.

**Source:** [clawdata/clawdata/skills/spark/SKILL.md](https://github.com/clawdata/clawdata/blob/f17377eaee1454a2d7a25b6e85d2b5de8dadf82d/skills/spark/SKILL.md) · 25★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: spark
description: "Build and run Apache Spark jobs -- submit applications, run interactive queries, manage data processing pipelines."
metadata: {"openclaw": {"emoji": "⚡", "requires": {"bins": ["spark-submit"]}, "tags": ["processing", "spark", "big-data", "etl", "data"]}}
---

# Apache Spark

You help build and run Apache Spark data processing jobs.
Use this when the user asks about Spark applications, DataFrame operations, SQL queries on Spark, or cluster management.

## Commands

### Submit a Spark application

```bash
spark-submit --master local[*] <script.py>
```

### Submit with dependencies

```bash
spark-submit --master local[*] --packages org.apache.spark:spark-avro_2.12:3.5.0 <script.py>
```

### Start PySpark shell

```bash
pyspark --master local[*]
```

### Start Spark SQL shell

```bash
spark-sql --master local[*]
```

## PySpark Patterns

### Read and write data

```python
from pyspark.sql import SparkSession

spark = SparkSession.builder.appName("my_app").getOrCreate()

# Read
df = spark.read.parquet("s3a://bucket/path/")
df = spark.read.csv("data/input.csv", header=True, inferSchema=True)
df = spark.read.json("data/events.json")

# Write
df.write.parquet(
```

</details>
