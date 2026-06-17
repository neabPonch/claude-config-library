---
name: chdb-io__chdb__skill
source: https://github.com/chdb-io/chdb/blob/e8d4b9171b8a89e12f37fb45ac07f76a5d5e6017/agent/skills/chdb-datastore/SKILL.md
repo: chdb-io/chdb
kind: skill
stars: 2694
last_pushed: 2026-06-10T02:30:48Z
license: apache-2.0
score: 9
domains: [data-engineering, cli-tools, python]
tags: [pandas-replacement, olap, sql-engine]
curated: 2026-06-15
curated_by: config-scout
---

# chdb-io/chdb — skill

**Why it's worth keeping:** Uses excellent 'Decision Tree' logic for intent classification and includes a specific 'Troubleshooting' table for error recovery, which is vital for agent autonomy.

**Summary:** A highly specialized skill file that instructs an agent on how to use chDB's DataStore API as a high-performance replacement for pandas. It excels at explaining cross-source joins and lazy execution patterns.

**Source credibility:** Highly credible; sourced from an active, high-star open-source project (chDB).

**Recency:** Current; follows modern agentic patterns of explicit trigger/skip logic and tool-specific context.

**Source:** [chdb-io/chdb/agent/skills/chdb-datastore/SKILL.md](https://github.com/chdb-io/chdb/blob/e8d4b9171b8a89e12f37fb45ac07f76a5d5e6017/agent/skills/chdb-datastore/SKILL.md) · 2694★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: chdb-datastore
description: >-
  Use when the user has tabular data (pandas DataFrame, parquet, csv,
  Arrow, json) and wants to filter, group, aggregate, join, or speed
  up slow pandas. Provides chDB DataStore — same pandas API,
  ClickHouse engine underneath. Also handles reading from S3, MySQL,
  PostgreSQL, MongoDB, ClickHouse Cloud, Iceberg, Delta Lake as
  DataFrames and joining across sources.
  TRIGGER when: user mentions DataFrame, parquet, csv, "fast pandas",
  "speed up pandas", or cross-source DataFrame joins; user imports
  `chdb.datastore` or `from datastore import DataStore`.
  SKIP this skill for raw SQL syntax (use chdb-sql instead),
  ClickHouse server administration, or non-Python DataStore API work.
license: Apache-2.0
compatibility: Requires Python 3.9+, macOS or Linux. pip install chdb.
metadata:
  author: chdb-io
  version: "4.1"
  homepage: https://clickhouse.com/docs/chdb
---

# chdb DataStore — It's Just Faster Pandas

## The Key Insight

```python
# Change this:
import pandas as pd
# To this:
import chdb.datastore as pd
# Everything else stays the same.
```

DataStore is a **lazy, ClickHouse-backed pandas replacement**. Your existing pandas cod
```

</details>
