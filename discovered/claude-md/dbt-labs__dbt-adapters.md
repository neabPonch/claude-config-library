---
name: dbt-labs__dbt-adapters
source: https://github.com/dbt-labs/dbt-adapters/blob/d6de330577d589fa12f210fb2264d6f5c6a21d51/CLAUDE.md
repo: dbt-labs/dbt-adapters
kind: claude-md
stars: 215
last_pushed: 2026-06-12T14:14:06Z
license: apache-2.0
score: 9
domains: [data-engineering, python, monorepo]
tags: [dbt, database-adapters, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# dbt-labs/dbt-adapters — claude-md

**Why it's worth keeping:** It provides exact CLI command mappings, clear architectural hierarchy, and specific code patterns (testing/macros) that allow an AI to navigate and contribute to a large-scale codebase without ambiguity.

**Summary:** A highly structured technical guide for a complex monorepo involving multiple database adapters.

**Source credibility:** High; dbt Labs is a standard-setter in data engineering with high star counts and active development.

**Recency:** Current; utilizes modern Python tooling like hatch and reflects recent database features.

**Source:** [dbt-labs/dbt-adapters/CLAUDE.md](https://github.com/dbt-labs/dbt-adapters/blob/d6de330577d589fa12f210fb2264d6f5c6a21d51/CLAUDE.md) · 215★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# dbt Adapters — Development Guide

## Monorepo Structure

```
dbt-adapters/
├── dbt-adapters/          # Base framework and protocols
├── dbt-tests-adapter/     # Reusable test suite
├── dbt-postgres/          # PostgreSQL adapter (base for redshift)
├── dbt-redshift/          # Amazon Redshift adapter (extends postgres)
├── dbt-snowflake/         # Snowflake adapter
├── dbt-bigquery/          # Google BigQuery adapter
├── dbt-spark/             # Apache Spark / Databricks adapter
├── dbt-athena/            # AWS Athena adapter
└── .pre-commit-config.yaml
```

Dependency chain:
```
dbt-adapters (base)
├── dbt-postgres
│   └── dbt-redshift
├── dbt-snowflake
├── dbt-bigquery
├── dbt-spark
└── dbt-athena

dbt-tests-adapter → used by all adapters for testing
```

## Development Workflow

All commands run from the specific adapter directory (e.g. `cd dbt-redshift`).

```shell
# Prerequisites
pip install hatch changie pre-commit

# Initial setup (installs adapter + deps in editable mode)
hatch run setup

# Code quality (Black, Flake8, MyPy)
hatch run code-quality

# Unit tests (no database required)
hatch run unit-tests
hatch run unit-tests -- tests/unit/test_file.py::TestClass::test_me
```

</details>
