---
name: databricks__tmm__claude
source: https://github.com/databricks/tmm/blob/fde6d524c66472472bc032ae7779bdc063179c48/OSS-SDP-HelloWorld/CLAUDE.md
repo: databricks/tmm
kind: claude-md
stars: 263
last_pushed: 2026-06-03T11:56:55Z
license: other
score: 9
domains: [data-engineering, apache-spark, cli-tools]
tags: [spark, pyspark, environment-config, state-management]
curated: 2026-06-15
curated_by: config-scout
---

# databricks/tmm — claude-md

**Why it's worth keeping:** The 'Architectural decisions' section provides specific 'gotchas' (Java 21+ breaking changes, SparkConnect scope issues) that prevent an AI from suggesting standard but broken solutions. It also includes a comprehensive 'reset story' for managing runtime state.

**Summary:** Provides essential setup commands alongside deep architectural context for running Spark pipelines locally. It explicitly details environmental nuances like Java version requirements and Spark session constraints.

**Source credibility:** High; written by Databricks, the industry leader in Spark-based engineering.

**Recency:** Very current; utilizes modern tooling like `uv` and addresses recent Java/Spark compatibility issues.

**Source:** [databricks/tmm/OSS-SDP-HelloWorld/CLAUDE.md](https://github.com/databricks/tmm/blob/fde6d524c66472472bc032ae7779bdc063179c48/OSS-SDP-HelloWorld/CLAUDE.md) · 263★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Commands

```bash
uv venv --python 3.11 --seed
uv pip install --offline -r requirements.txt  # drop --offline if not cached

./run_pipeline.sh    # run the pipeline
./show_output.sh     # inspect results (no JVM needed)
./reset.sh           # wipe all runtime state for a clean restart
```

## What this project is

A minimal OSS Apache Spark Declarative Pipelines (SDP) example. It was built by adapting the reference project at [databricks/tmm/OSS-SDP-OpenSkyNetwork](https://github.com/databricks/tmm/tree/main/OSS-SDP-OpenSkyNetwork) to use local JSON files instead of the OpenSky live API, making it fully self-contained and runnable offline.

The pipeline has two steps:
- `transformations/ingest.py` — streaming table, reads JSON events
- `transformations/aggregate.sql` — materialized view, counts by event type

## Architectural decisions and how we got there

### Java 17 (not system Java)

Running `spark-pipelines run` on Java 25 fails immediately with `UnsupportedOperationException: getSubject is not supported`. The cause: Java 21+ removed `javax.security.auth.Subject.getSubject()`, which Hadoop's `UserGroupInformation` still calls at startup. Spark 4.x is tested aga
```

</details>
