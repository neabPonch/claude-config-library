---
name: CSenshi__pg_grpc__skill
source: https://github.com/CSenshi/pg_grpc/blob/0d56147497ee75cbe5b508ca99cfa6b3500f1d78/website/static/skill.md
repo: CSenshi/pg_grpc
kind: skill
stars: 28
last_pushed: 2026-05-04T22:40:34Z
license: mit
score: 9
domains: [database, backend-api, grpc]
tags: [postgresql, grpc, extension, rpc]
curated: 2026-06-15
curated_by: config-scout
---

# CSenshi/pg_grpc — skill

**Why it's worth keeping:** Provides highly specific error prefix mappings and complex JSONB options (TLS/mTLS) that allow an agent to perform precise debugging and orchestration.

**Summary:** Technical specification for the pg_grpc extension, enabling unary gRPC calls directly from PostgreSQL SQL queries.

**Source credibility:** High; detailed, structured technical documentation for a specialized database extension.

**Recency:** Very current; updated within the last month.

**Source:** [CSenshi/pg_grpc/website/static/skill.md](https://github.com/CSenshi/pg_grpc/blob/0d56147497ee75cbe5b508ca99cfa6b3500f1d78/website/static/skill.md) · 28★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pg_grpc
description: Make gRPC calls from PostgreSQL SQL queries using the pg_grpc extension
---

# pg_grpc

pg_grpc is a PostgreSQL extension (Postgres 13–18) that lets you invoke unary gRPC methods directly from a SQL query — no sidecar, no codegen, no application layer.

## When to use

- Call a gRPC service from inside a SQL query, trigger, or function
- Join gRPC service responses with database rows in one query
- Invoke an external service within a Postgres transaction
- Test a gRPC endpoint interactively from psql

## Setup

```sql
CREATE EXTENSION IF NOT EXISTS pg_grpc;
```

## Core function

```sql
grpc_call(
  endpoint TEXT,                  -- host:port — no http:// prefix
  method   TEXT,                  -- fully-qualified: pkg.Service/Method
  request  JSONB,                 -- request payload as JSON
  metadata JSONB DEFAULT NULL,    -- optional gRPC headers
  options  JSONB DEFAULT NULL     -- optional transport config
) RETURNS JSONB
```

## Quick patterns

**Server exposes gRPC reflection (most common):**
```sql
SELECT grpc_call(
  'localhost:50051',
  'auth.AuthService/GetUser',
  '{"id": "42"}'::jsonb
);
```

**User-supplied proto (server has no reflec
```

</details>
