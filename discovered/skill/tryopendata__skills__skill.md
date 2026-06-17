---
name: tryopendata__skills__skill
source: https://github.com/tryopendata/skills/blob/0f7c63b23e20cb2e8bdcb219c5ba024a9513b9e2/plugins/opendata/skills/opendata-api/SKILL.md
repo: tryopendata/skills
kind: skill
stars: 93
last_pushed: 2026-05-20T20:36:34Z
license: mit
score: 8
domains: [backend-api, data-science, agents-ai]
tags: [api-reference, mcp-first, data-analysis]
curated: 2026-06-16
curated_by: config-scout
---

# tryopendata/skills — skill

**Why it's worth keeping:** It includes specific tool-use hierarchy (MCP vs. REST) and 'negative constraints' to prevent common API misuse errors.

**Summary:** A highly structured API reference that provides clear instruction on authentication, endpoint schemas, and data retrieval patterns.

**Source credibility:** High; appears to be professional documentation for the OpenData platform.

**Recency:** Current; incorporates modern MCP (Model Context Protocol) prioritization logic.

**Source:** [tryopendata/skills/plugins/opendata/skills/opendata-api/SKILL.md](https://github.com/tryopendata/skills/blob/0f7c63b23e20cb2e8bdcb219c5ba024a9513b9e2/plugins/opendata/skills/opendata-api/SKILL.md) · 93★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: opendata-api
description: Query the OpenData API for data research and analysis. Use when fetching dataset rows, filtering, sorting, aggregating, inspecting columns, composing cross-dataset joins, exploring graph intelligence, or building data pipelines against OpenData endpoints.
---

# OpenData Query API

Query datasets stored as Parquet files through a REST API backed by DuckDB. The API returns JSON by default, with support for CSV, TSV, and XLSX exports.

**Base URL:** `https://api.tryopendata.ai` (production) or `http://localhost:8000` (local dev). Default to use production

## Authentication

All endpoints require authentication in production. Pass an API key via `Authorization: Bearer` header:

```bash
curl -H "Authorization: Bearer ${OPENDATA_API_KEY}" \
  "https://api.tryopendata.ai/v1/datasets/fred/cpi?limit=5"
```

Local dev (`localhost:8000`) does not require auth when running the standalone opendata server (`make quickstart`). The backend server (`make dev-all`) requires auth for write endpoints but allows unauthenticated reads.

## Quick Start

**For analysis (aggregations, joins, window functions), use SQL:**

```bash
# Average CPI by year, most recent firs
```

</details>
