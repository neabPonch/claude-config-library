---
name: apache__hamilton__skill
source: https://github.com/apache/hamilton/blob/6c05041d687db55f773b2d059e4ff794d0ec9118/.claude-plugin/skills/integrations/SKILL.md
repo: apache/hamilton
kind: skill
stars: 2526
last_pushed: 2026-06-14T09:23:14Z
license: apache-2.0
score: 8
domains: [data-engineering, backend-api, orchestration]
tags: [hamilton, airflow, dagster, fastapi, integration-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# apache/hamilton — skill

**Why it's worth keeping:** The examples include sophisticated production-ready patterns like XCom passing in Airflow, async driver initialization in FastAPI, and state management in Streamlit.

**Summary:** Provides concrete implementation patterns for integrating Hamilton dataflows with orchestrators (Airflow, Dagster) and serving/visualizing them via FastAPI and Streamlit.

**Source credibility:** High; based on a highly-starred Apache open-source project used widely in production data pipelines.

**Recency:** 

**Source:** [apache/hamilton/.claude-plugin/skills/integrations/SKILL.md](https://github.com/apache/hamilton/blob/6c05041d687db55f773b2d059e4ff794d0ec9118/.claude-plugin/skills/integrations/SKILL.md) · 2526★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: hamilton-integrations
description: Hamilton integration patterns for Airflow, Dagster, FastAPI, Streamlit, Jupyter notebooks, and other frameworks. Use when integrating Hamilton with other tools.
allowed-tools: Read, Grep, Glob, Bash(python:*), Bash(jupyter:*)
user-invocable: true
disable-model-invocation: false
---
<!-- SPDX-License-Identifier: Apache-2.0 -->

# Hamilton Integrations

This skill covers integrating Hamilton with orchestrators, web frameworks, notebooks, and other tools.

## Why Integrate Hamilton?

Hamilton focuses on **dataflow definition**, letting you integrate with:
- **Orchestrators** (Airflow, Dagster, Prefect) - Schedule and monitor
- **Web frameworks** (FastAPI, Flask) - Serve predictions
- **Dashboards** (Streamlit, Plotly Dash) - Interactive visualization
- **Notebooks** (Jupyter) - Interactive development
- **Experiment tracking** (MLflow, Weights & Biases) - Track experiments

## Airflow Integration

**Use Case:** Schedule Hamilton DAGs as Airflow tasks

```python
"""Hamilton in Airflow DAG."""
from airflow import DAG
from airflow.operators.python import PythonOperator
from datetime import datetime, timedelta
from hamilton import driver
import
```

</details>
