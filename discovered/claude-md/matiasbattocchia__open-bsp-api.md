---
name: matiasbattocchia__open-bsp-api
source: https://github.com/matiasbattocchia/open-bsp-api/blob/511bec2a318bb078b7b75e5dc7fc52a7c9c1d5df/CLAUDE.md
repo: matiasbattocchia/open-bsp-api
kind: claude-md
stars: 344
last_pushed: 2026-06-11T19:33:18Z
license: unlicense
score: 9
domains: [backend-api, cloud-infrastructure, devops]
tags: [supabase, edge-functions, debugging, database-migrations]
curated: 2026-06-14
curated_by: config-scout
---

# matiasbattocchia/open-bsp-api — claude-md

**Why it's worth keeping:** Includes a vital 'time-sync' tip to prevent timestamp hallucinations; provides ready-to-run curl/SQL templates that allow an agent to autonomously investigate remote errors.

**Summary:** Provides highly specific terminal commands and SQL snippets for debugging remote Supabase edge functions and production logs.

**Source credibility:** Strong: 344 stars and recent activity suggest a high-quality, production-ready codebase.

**Recency:** Very current; it addresses the specific observability challenges of using AI agents with serverless cloud environments.

**Source:** [matiasbattocchia/open-bsp-api/CLAUDE.md](https://github.com/matiasbattocchia/open-bsp-api/blob/511bec2a318bb078b7b75e5dc7fc52a7c9c1d5df/CLAUDE.md) · 344★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project overview

Open BSP API — a multi-tenant WhatsApp Business Platform integration built with
Deno, Postgres, and Supabase Edge Functions. See README.md for full details.

## Debugging production edge functions

### Timestamps

The current date/time is NOT reliably in the conversation context. When querying
logs with time ranges (e.g., "last 12 hours"), **always run `date -u` first** to
get the actual current UTC time. Do not guess or hardcode timestamps.

### Querying stdout logs (console.log / console.error)

Use the Supabase Management API to query `function_logs` (edge function stdout):

```bash
ACCESS_TOKEN=$(cat ~/.supabase/access-token)
REF="nheelwshzbgenpavwhcy"

curl -s "https://api.supabase.com/v1/projects/${REF}/analytics/endpoints/logs.all" \
  -H "Authorization: Bearer ${ACCESS_TOKEN}" \
  -G \
  --data-urlencode "sql=select cast(timestamp as datetime) as ts, event_message from function_logs where regexp_contains(event_message, 'ERROR_KEYWORD') order by timestamp desc limit 10" \
  --data-urlencode "iso_timestamp_start=2026-04-10T00:00:00Z"
```

Available log tables: `function_logs` (stdout), `function_edge_logs`
(HTTP-level), `edge_logs`, `postgres
```

</details>
