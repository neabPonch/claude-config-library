---
name: sapporo-wes__sapporo-service__agent-skill
source: https://github.com/sapporo-wes/sapporo-service/blob/096022ad7e827ead53038100eab9be5ecac33508/docs/agent-skill.md
repo: sapporo-wes/sapporo-service
kind: skill
stars: 25
last_pushed: 2026-04-16T01:55:02Z
license: apache-2.0
score: 9
domains: [bioinformatics, cli-tools, api-integration, workflow-automation]
tags: [wes, api, shell, bioinformatics]
curated: 2026-06-15
curated_by: config-scout
---

# sapporo-wes/sapporo-service — skill

**Why it's worth keeping:** It provides production-ready shell patterns including automated polling loops with state machine awareness and jq-integrated command chains.

**Summary:** A highly structured operational guide for interacting with the Sapporo WES API via shell commands.

**Source credibility:** The repository implements a recognized industry standard (GA4GH WES) with stable maintenance history.

**Recency:** Very current; uses modern CLI tools like jq and follows standard API interaction patterns used by modern agents.

**Source:** [sapporo-wes/sapporo-service/docs/agent-skill.md](https://github.com/sapporo-wes/sapporo-service/blob/096022ad7e827ead53038100eab9be5ecac33508/docs/agent-skill.md) · 25★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Sapporo WES Agent Skill

LLM agent reference for running bioinformatics workflows via Sapporo WES using `curl`.

For the full request/response schema, see [`openapi/sapporo-wes-spec-2.1.0.yml`](../openapi/sapporo-wes-spec-2.1.0.yml) or the interactive docs at `$SAPPORO_ENDPOINT/docs`.

> **Tight on context?** Use [`docs/agent-quick-ref.md`](agent-quick-ref.md) — the essential 4 commands in ~40 lines.

## Prerequisites

- `curl` and `jq`
- `SAPPORO_ENDPOINT` set to the base URL (default: `http://localhost:1122`)

## Phase 0: Start a local server (if needed)

```bash
curl -s $SAPPORO_ENDPOINT/service-info | jq .workflow_engine_versions
```

If that fails, start with Docker Compose:

```bash
curl -O https://raw.githubusercontent.com/sapporo-wes/sapporo-service/main/compose.yml
docker compose up -d
```

## Phase 1: Submit a workflow

`POST /runs` accepts `application/json` (remote files) or `multipart/form-data` (local file upload). For the full list of fields and types, see the OpenAPI spec. The four required fields are `workflow_type`, `workflow_type_version`, `workflow_url`, and `workflow_engine`.

To find what engines and types your server supports:

```bash
curl -s $SAPPORO_ENDP
```

</details>
