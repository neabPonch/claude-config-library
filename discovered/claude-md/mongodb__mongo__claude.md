---
name: mongodb__mongo__claude
source: https://github.com/mongodb/mongo/blob/831a146d652c2e3d795ee4362951aea394dda28a/src/mongo/db/extension/CLAUDE.md
repo: mongodb/mongo
kind: claude-md
stars: 28365
last_pushed: 2026-06-12T08:32:38Z
license: other
score: 9
domains: [backend, systems-programming, database-internals]
tags: [architecture, abi-stability, c-api, mongodb]
curated: 2026-06-15
curated_by: config-scout
---

# mongodb/mongo — claude-md

**Why it's worth keeping:** The 'Common Mistakes' section is a perfect template for preventing subtle architectural violations (e.g., exception escaping or type boundary errors). The use of an ASCII architecture diagram and navigation tables provides excellent context for AI agents.

**Summary:** Defines the architecture, ABI constraints, and lifecycle of the MongoDB Extensions API. It provides rigorous rules for safe C-boundary interactions between C++ and Rust.

**Source credibility:** Extremely high; official technical specification from the MongoDB core repository.

**Recency:** Very recent, reflecting active development.

**Source:** [mongodb/mongo/src/mongo/db/extension/CLAUDE.md](https://github.com/mongodb/mongo/blob/831a146d652c2e3d795ee4362951aea394dda28a/src/mongo/db/extension/CLAUDE.md) · 28365★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Extensions API

The MongoDB Extensions API is a dynamic plugin system that loads shared libraries (`.so` files) into
the server at startup to provide additional aggregation stages. Extensions are developed, versioned,
and deployed independently of the server. The primary use case is moving Atlas Search stages
(`$vectorSearch`, `$search`, `$searchMeta`) out of the server codebase. Only Rust extensions are
supported in production; the C++ SDK here is for internal testing.

### Architecture

```
┌─────────────────────────┐    ┌──────────────────────────┐
│     Host Logic          │    │   Extension Code         │
│  (mongo::extension::    │    │  (Rust in prod,          │
│   host)                 │    │   C++ for tests)         │
├─────────────────────────┤    ├──────────────────────────┤
│   Host Connector        │    │       C++ SDK            │
│  (mongo::extension::    │    │  (mongo::extension::     │
│   host_connector)       │    │   sdk)                   │
├─────────────────────────┴────┴──────────────────────────┤
│              Public C API  (public/api.h)               │
│         Stable ABI - vtable-based polymorphism          │
└──────────────────────────────────────
```

</details>
