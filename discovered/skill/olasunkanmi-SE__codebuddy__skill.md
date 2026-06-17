---
name: olasunkanmi-SE__codebuddy__skill
source: https://github.com/olasunkanmi-SE/codebuddy/blob/f921c335c03b6e6b4287c14411f161105b207279/skills/elasticsearch/SKILL.md
repo: olasunkanmi-SE/codebuddy
kind: skill
stars: 132
last_pushed: 2026-05-01T03:21:24Z
license: mit
score: 7
domains: [databases, cli-tools, backend]
tags: [elasticsearch, api, database]
curated: 2026-06-15
curated_by: config-scout
---

# olasunkanmi-SE/codebuddy — skill

**Why it's worth keeping:** It excels at defining machine-readable metadata like system dependencies (curl) and configuration variables (ES_URL), which is critical for autonomous environment setup.

**Summary:** Provides a structured template for interacting with Elasticsearch via API, including environmental requirements and configuration schemas.

**Source credibility:** Moderate; 132 stars suggests a useful but niche open-source toolset.

**Recency:** Current, as it relies on standard CLI/REST patterns used in modern agentic workflows.

**Source:** [olasunkanmi-SE/codebuddy/skills/elasticsearch/SKILL.md](https://github.com/olasunkanmi-SE/codebuddy/blob/f921c335c03b6e6b4287c14411f161105b207279/skills/elasticsearch/SKILL.md) · 132★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: elasticsearch
description: Interact with Elasticsearch clusters via the API.
metadata:
  displayName: Elasticsearch
  icon: search
  category: databases
  version: 1.0.0
  dependencies:
    cli: curl
    checkCommand: curl --version
    bundledInstall: skills/elasticsearch/install.sh
    install:
      darwin:
        brew: curl
      linux:
        apt: curl
        dnf: curl
      windows:
        scoop: curl
        choco: curl
  config:
    - name: ES_URL
      label: Base URL
      type: string
      required: false
      placeholder: http://localhost:9200
  auth:
    type: api-key
---

# Elasticsearch

Use the provided `es-cli` wrapper or direct REST API calls to manage indexes and search data.

## CLI Usage (Recommended)

An `es-cli` wrapper is available in `.codebuddy/bin`.

Base URL default: `http://localhost:9200` (Override with ES_URL env var)

### Examples

- Check Health: `es-cli GET /_cluster/health`
- List Indexes: `es-cli GET /_cat/indices`
- Search: `es-cli GET /my-index/_search`

## Manual Connection

Typically accessed via `curl`.
Base URL: `http://localhost:9200` (or your cluster URL)

## Common Commands

### Cluster Health

```bash
curl -X GET "localh
```

</details>
