---
name: orneryd__NornicDB__grpc-skill
source: https://github.com/orneryd/NornicDB/blob/41372f7aa4810c7bc87c2b815be9bd25df3acbe3/docs/skills/grpc.skill.md
repo: orneryd/NornicDB
kind: skill
stars: 773
last_pushed: 2026-06-15T18:58:14Z
license: mit
score: 9
domains: [backend-api, databases, distributed-systems]
tags: [grpc, vector-database, migration, hybrid-search]
curated: 2026-06-15
curated_by: config-scout
---

# orneryd/NornicDB — skill

**Why it's worth keeping:** The inclusion of explicit data model mapping (e.g., Qdrant concepts to internal storage details) and a protocol decision matrix provides an excellent template for teaching agents how to handle migrations or multi-protocol environments.

**Summary:** A highly structured technical specification for the NornicDB gRPC interface, detailing Qdrant compatibility and custom search services.

**Source credibility:** High; the repository is actively maintained with significant community interest/stars.

**Recency:** Extremely current, as indicated by recent push activity.

**Source:** [orneryd/NornicDB/docs/skills/grpc.skill.md](https://github.com/orneryd/NornicDB/blob/41372f7aa4810c7bc87c2b815be9bd25df3acbe3/docs/skills/grpc.skill.md) · 773★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: nornicdb-grpc
description: Drive NornicDB over gRPC — the Qdrant-compatible surface (Collections, Points, Snapshots) plus the additive NornicSearch service. Use when ingesting via Qdrant SDKs, migrating from Qdrant, or running hybrid text+vector search from a non-Bolt client. Covers connection, RPC catalog, collection→database mapping, point→node mapping, limits, auth, and minimum-viable client examples.
---

# NornicDB gRPC (Qdrant + NornicSearch)

NornicDB exposes two gRPC services on the same listener:

1. **Qdrant compatibility** — full set of `qdrant.Collections`, `qdrant.Points`, and `qdrant.Snapshots` services. Existing Qdrant SDKs work without modification.
2. **`NornicSearch`** — one additive RPC, `SearchText`, that returns hybrid (vector + BM25 + RRF) results.

The same client connection talks to both; pick whichever matches the operation.

## Connection

| Setting | Value |
|---|---|
| Listen address | `:6334` (`NORNICDB_QDRANT_GRPC_LISTEN_ADDR`) |
| Default port (host) | `6334` |
| Auth | Same `Auth.Enabled` flag as Bolt. When off, gRPC is open. When on, basic auth or bearer JWT in the gRPC metadata. |
| TLS | None by default (run behind a TLS proxy or in a pr
```

</details>
