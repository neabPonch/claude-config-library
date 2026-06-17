---
name: dr4gon123__flasi
source: https://github.com/dr4gon123/flasi/blob/a570b6179707985ad70ecbd7c0348940ec16a6c9/CLAUDE.md
repo: dr4gon123/flasi
kind: claude-md
stars: 109
last_pushed: 2026-06-05T01:15:32Z
license: apache-2.0
score: 9
domains: [security, data-engineering, devops]
tags: [log-ingestion, etl, observability, security-analytics]
curated: 2026-06-16
curated_by: config-scout
---

# dr4gon123/flasi — claude-md

**Why it's worth keeping:** The 'FortiGate Log Quirks' section provides critical domain-specific edge cases (e.g., handling 'N/A' values and type conflicts) that prevent common ETL errors. It also demonstrates an advanced pattern of using distributed CLAUDE.md files for component-specific context.

**Summary:** A technical specification for a security log analytics platform detailing data flows, mapping philosophies, and component-specific instructions.

**Source credibility:** High; the repo has significant stars (109) and is very actively maintained.

**Recency:** Extremely current, with updates within the last month.

**Source:** [dr4gon123/flasi/CLAUDE.md](https://github.com/dr4gon123/flasi/blob/a570b6179707985ad70ecbd7c0348940ec16a6c9/CLAUDE.md) · 109★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

FLASI is a full analytics platform for threat hunting with Fortinet datasources. It integrates Fortinet logs (FortiGate, FortiEDR, FortiMail, FortiWeb) and Palo Alto PAN-OS logs with multiple storage backends (Elasticsearch, Victoria Logs) and visualization platforms (Kibana, Grafana).

**Key Architecture Principle**: Modular design with decoupled layers — data sources, ingestion, storage, and visualization are independent and swappable.

Each component has its own `CLAUDE.md` with component-specific commands and gotchas:
- [`vector/CLAUDE.md`](vector/CLAUDE.md) — Vector.dev ingestion pipelines and VRL transforms
- [`ELK/CLAUDE.md`](ELK/CLAUDE.md) — Elasticsearch index templates, ingest pipelines, Kibana dashboards
- [`grafana/CLAUDE.md`](grafana/CLAUDE.md) — Grafana dashboards (JSON + future SDK)
- [`docs/CLAUDE.md`](docs/CLAUDE.md) — MkDocs documentation site

## Repository Structure

```
vector/          # Vector ingestion pipelines (recommended ingestion method)
ELK/             # Elasticsearch configuration: templates, pipelines, Kibana dashboards
grafana/         # Grafana dashboard JSON files, organized by datasource
docs/            # MkDocs documentation sourc
```

</details>
