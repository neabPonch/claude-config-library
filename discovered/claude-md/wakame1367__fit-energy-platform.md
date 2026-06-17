---
name: wakame1367__fit-energy-platform
source: https://github.com/wakame1367/fit-energy-platform/blob/13a6e525a83630ea6d830f29227f548951b82594/Claude.md
repo: wakame1367/fit-energy-platform
kind: claude-md
stars: 0
last_pushed: 2025-07-27T14:14:02Z
license: mit
score: 8
domains: [data-pipeline, infrastructure-as-code, serverless]
tags: [architecture, terraform, security-permissions, workflow]
curated: 2026-06-16
curated_by: config-scout
---

# wakame1367/fit-energy-platform — claude-md

**Why it's worth keeping:** Includes explicit 'Tool Permissions' to prevent unauthorized infra changes and provides highly specific operational context like S3 naming patterns.

**Summary:** Defines a complex data/infra pipeline with clear architectural boundaries and command sets.

**Source credibility:** Low (0-star personal project), but content density is high.

**Recency:** Current; explicitly references Claude Code interaction modes and content reference syntax.

**Source:** [wakame1367/fit-energy-platform/Claude.md](https://github.com/wakame1367/fit-energy-platform/blob/13a6e525a83630ea6d830f29227f548951b82594/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# 🚀 Project Overview
This repository implements a lightweight solar FIT-pipeline:
- Download monthly FIT Excel → parse to CSV → geocode → convert to GeoParquet.
- Data stored in S3; DuckDB used for querying and dashboard.
- Apps: frontend (Next.js + Mapbox + DuckDB‑WASM), API (Lambda), data pipeline (Lambda ETL).
- Infra managed with Terraform modules (`lambda`, `s3`, `eventbridge`, etc.).

# 🔧 Common Commands
- `make infra-dev apply` / `make infra-prod apply` – Deploy Terraform in respective envs.
- `make run-local-pipeline` – Run Excel-to-GeoParquet flow locally.
- `make test` – Run tests across packages.
- `make lint` – Code formatting and linting.

# 🧰 Code Style & Structure
- Terraform modules under `modules/terraform/*`.
- Apps under `apps/{frontend, api, data_pipeline}`.
- Use snake_case for filenames/scripts, PascalCase for components.
- Use Prettier / ESLint / black for formatting.

# 🧵 Workflow
1. Read and understand context: don't edit before planning.
2. Use agentic cycle: **think → plan → code → test → commit**.
3. Tests (DuckDB queries or Lambda integration) must pass before commit.
4. Frequent small PRs; request ≥2 reviews before merge.
5. Clear commit messages (e.g.
```

</details>
