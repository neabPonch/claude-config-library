---
name: neo4j-contrib__neo4j-skills__skill
source: https://github.com/neo4j-contrib/neo4j-skills/blob/6d44d3166bf888ac4fc294b88c72df6d1d83abcb/neo4j-spark-skill/SKILL.md
repo: neo4j-contrib/neo4j-skills
kind: skill
stars: 83
last_pushed: 2026-06-09T15:33:47Z
license: mit
score: 9
domains: [data-engineering, database, big-data]
tags: [neo4j, apache-spark, databricks, pyspark, scala]
curated: 2026-06-16
curated_by: config-scout
---

# neo4j-contrib/neo4j-skills — skill

**Why it's worth keeping:** Includes critical 'When NOT to Use' boundaries to prevent tool confusion, plus production-ready patterns like deadlock prevention via coalesce(1) and Databricks secret handling.

**Summary:** A high-density technical reference for using the Neo4j connector with Apache Spark and Databricks.

**Source credibility:** Official/high-quality community contribution from neo4j-contrib with active maintenance.

**Recency:** Extremely current, featuring 2025 versions and modern Spark/Databricks configurations.

**Source:** [neo4j-contrib/neo4j-skills/neo4j-spark-skill/SKILL.md](https://github.com/neo4j-contrib/neo4j-skills/blob/6d44d3166bf888ac4fc294b88c72df6d1d83abcb/neo4j-spark-skill/SKILL.md) · 83★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: neo4j-spark-skill
description: Use when reading from or writing to Neo4j with Apache Spark or Databricks using the
  Neo4j Connector for Apache Spark (org.neo4j:neo4j-connector-apache-spark). Covers SparkSession
  setup, DataFrame reads via labels/Cypher/relationship scan, DataFrame writes with SaveMode,
  node.keys for MERGE, relationship write mapping, partition and batch tuning, PySpark and Scala
  examples, Databricks cluster config, Databricks secrets for credentials, Delta Lake to Neo4j
  pipelines. Does NOT handle Cypher authoring — use neo4j-cypher-skill. Does NOT handle the Python
  bolt driver — use neo4j-driver-python-skill. Does NOT handle GDS algorithms — use neo4j-gds-skill.
version: 1.0.1
allowed-tools: Bash WebFetch
---

# Neo4j Connector for Apache Spark

## When to Use

- Reading Neo4j nodes/relationships into Spark DataFrames
- Writing Spark DataFrames to Neo4j as nodes or relationships
- Databricks notebooks connecting to Neo4j
- Delta Lake → Neo4j ingestion pipelines
- Partitioned parallel reads from large Neo4j graphs

## When NOT to Use

- **Python bolt driver / execute_query** → `neo4j-driver-python-skill`
- **Cypher query writing** → `neo4j-cypher
```

</details>
