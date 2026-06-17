---
name: acryldata__datahub-helm
source: https://github.com/acryldata/datahub-helm/blob/e42fb9522a53399c6b72cf63affeaa384c09269d/CLAUDE.md
repo: acryldata/datahub-helm
kind: claude-md
stars: 204
last_pushed: 2026-06-15T15:13:07Z
license: apache-2.0
score: 7
domains: [devops, infrastructure]
tags: [helm, configuration-patterns, kubernetes]
curated: 2026-06-16
curated_by: config-scout
---

# acryldata/datahub-helm — claude-md

**Why it's worth keeping:** Includes a specific 'Rule of thumb' that provides the AI with logical decision criteria rather than just a list of examples.

**Summary:** Defines a two-tier naming convention for Helm 'values.yaml' files to distinguish between external infrastructure and internal DataHub features.

**Source credibility:** DataHub is a highly-regarded, enterprise-grade metadata platform.

**Recency:** Current; aligns with modern Kubernetes/Helm configuration practices.

**Source:** [acryldata/datahub-helm/CLAUDE.md](https://github.com/acryldata/datahub-helm/blob/e42fb9522a53399c6b72cf63affeaa384c09269d/CLAUDE.md) · 204★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - DataHub Helm Chart

## values.yaml Naming Conventions

The `global` section in `charts/datahub/values.yaml` follows a two-tier naming convention:

### Infrastructure backends — directly under `global`

External infrastructure dependencies that DataHub connects to are placed directly
under `global.*`:

- `global.elasticsearch` — Elasticsearch/OpenSearch cluster configuration
- `global.kafka` — Kafka broker and topic configuration
- `global.neo4j` — Neo4j graph database configuration
- `global.sql` — SQL database (MySQL/PostgreSQL) configuration

### DataHub application features — under `global.datahub`

Configuration for DataHub application behavior and features lives under
`global.datahub.*`:

- `global.datahub.gms` — GMS service settings
- `global.datahub.monitoring` — Prometheus/monitoring settings
- `global.datahub.managed_ingestion` — UI ingestion feature
- `global.datahub.metadata_service_authentication` — Auth configuration
- `global.datahub.search_and_browse` — Search UI feature flags
- `global.datahub.semantic_search` — Semantic/vector search configuration
- `global.datahub.mcp` — Metadata Change Proposal throttling
- `global.datahub.encryptionKey` — Encryptio
```

</details>
