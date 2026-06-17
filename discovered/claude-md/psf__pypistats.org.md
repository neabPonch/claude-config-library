---
name: psf__pypistats.org
source: https://github.com/psf/pypistats.org/blob/751726e5b9d4128bdc5524b46572d4fd1ec4ac48/CLAUDE.md
repo: psf/pypistats.org
kind: claude-md
stars: 195
last_pushed: 2026-03-31T23:50:32Z
license: apache-2.0
score: 8
domains: [backend-api, data-pipeline, web-app]
tags: [flask, etl, analytics, bigquery]
curated: 2026-06-16
curated_by: config-scout
---

# psf/pypistats.org — claude-md

**Why it's worth keeping:** The detailed breakdown of the ETL lifecycle (BigQuery to Celery to PostgreSQL) is vital for an AI to understand complex background state changes.

**Summary:** An exhaustive architectural blueprint covering data pipelines, component interactions, and system configuration.

**Source credibility:** Established open-source project with significant stars and recent maintenance.

**Recency:** Recent updates ensure the tech stack remains relevant for modern development environments.

**Source:** [psf/pypistats.org/CLAUDE.md](https://github.com/psf/pypistats.org/blob/751726e5b9d4128bdc5524b46572d4fd1ec4ac48/CLAUDE.md) · 195★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# PyPIStats.org - Python Package Download Analytics

## Overview
PyPIStats.org is a Flask-based web application that provides analytics and visualization for Python package download statistics from PyPI (Python Package Index). It queries BigQuery public datasets, aggregates the data, and presents it through both a web interface and JSON API.

## Architecture

### Core Technologies
- **Framework**: Flask (Python web framework)
- **Database**: PostgreSQL for storing aggregated statistics
- **Task Queue**: Celery with Redis for background processing
- **Data Source**: Google BigQuery (bigquery-public-data.pypi.file_downloads)
- **Visualization**: Plotly.js for interactive charts
- **Authentication**: GitHub OAuth for user features
- **Deployment**: Docker/Kubernetes support included

## Key Components

### 1. Data Pipeline (`pypistats/tasks/pypi.py`)
- **ETL Process**: Daily scheduled task (1am UTC) via Celery
- **BigQuery Integration**: Queries PyPI public dataset for download statistics
- **Data Categories**:
  - Overall downloads (with/without mirrors)
  - Python major versions (2, 3)
  - Python minor versions (2.7, 3.6, etc.)
  - Operating systems (Windows, Linux, Darwin, other)
-
```

</details>
