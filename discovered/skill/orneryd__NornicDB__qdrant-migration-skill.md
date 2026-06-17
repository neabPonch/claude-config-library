---
name: orneryd__NornicDB__qdrant-migration-skill
source: https://github.com/orneryd/NornicDB/blob/41372f7aa4810c7bc87c2b815be9bd25df3acbe3/docs/skills/qdrant-migration.skill.md
repo: orneryd/NornicDB
kind: skill
stars: 773
last_pushed: 2026-06-15T18:58:14Z
license: mit
score: 9
domains: [backend-api, database-migration, data-engineering]
tags: [migration, qdrant, vector-db, grpc]
curated: 2026-06-16
curated_by: config-scout
---

# orneryd/NornicDB — skill

**Why it's worth keeping:** The 'Mapping Reference' (Concept $ightarrow$ Equivalent) and 'Cutover Playbook' are elite patterns for migration tasks. It also includes critical 'what does NOT transfer' warnings to prevent data loss expectations.

**Summary:** A technical skill for migrating vector data from Qdrant to NornicDB via gRPC. It covers configuration replication, point streaming/upserting, and verification processes.

**Source credibility:** High; the repository is actively maintained with zero-month recency and deep technical specifications.

**Recency:** Extremely current, utilizing modern gRPC/Protobuf patterns relevant to today's infrastructure.

**Source:** [orneryd/NornicDB/docs/skills/qdrant-migration.skill.md](https://github.com/orneryd/NornicDB/blob/41372f7aa4810c7bc87c2b815be9bd25df3acbe3/docs/skills/qdrant-migration.skill.md) · 773★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: nornicdb-qdrant-migration
description: Migrate from Qdrant to NornicDB end-to-end through NornicDB's Qdrant-compatible gRPC surface. Covers connection setup, collection→database mapping, point→node mapping, the vector-config and named-vector replication, point upsert in batches, count verification, and what (deliberately) does not transfer (snapshots, HNSW tuning, quantization). Points to runnable Python/Go/Node scripts.
---

# Migrating from Qdrant to NornicDB

NornicDB's Qdrant-compatible gRPC service means migration is a **same-API replay**: the source and target speak the same wire, so the script reading from Qdrant can write into NornicDB through the same client library. There is no protocol bridge to build, no schema translation to invent.

This skill covers the migration surface itself. Runnable scripts are in [`scripts/migration/qdrant/`](https://github.com/orneryd/nornicdb/tree/main/scripts/migration/qdrant).

## Prerequisites

1. **Enable the gRPC server on NornicDB.** Off by default:
   ```bash
   export NORNICDB_QDRANT_GRPC_ENABLED=true
   export NORNICDB_QDRANT_GRPC_LISTEN_ADDR=":6334"
   ```
2. **Match dimension limits.** If your source has vectors above `40
```

</details>
