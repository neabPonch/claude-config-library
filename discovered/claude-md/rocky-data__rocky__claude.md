---
name: rocky-data__rocky__claude
source: https://github.com/rocky-data/rocky/blob/2755030efe66aca500bafaa893769e99a9854ef6/engine/CLAUDE.md
repo: rocky-data/rocky
kind: claude-md
stars: 265
last_pushed: 2026-06-15T10:10:47Z
license: apache-2.0
score: 9
domains: [rust, data-engineering, compiler-design]
tags: [monorepo, architecture-mapping, high-context]
curated: 2026-06-15
curated_by: config-scout
---

# rocky-data/rocky — claude-md

**Why it's worth keeping:** It includes crucial 'evolutionary context' (e.g., the migration from Plan to ModelIr), which prevents an AI from attempting to use deprecated or removed patterns.

**Summary:** Provides a comprehensive architectural map of a complex Rust monorepo, detailing crate responsibilities and the internal data hierarchy.

**Source credibility:** Highly credible; a sophisticated, active Rust-based data engineering engine with high technical density.

**Recency:** Very current, referencing Rust edition 2024 and modern development standards.

**Source:** [rocky-data/rocky/engine/CLAUDE.md](https://github.com/rocky-data/rocky/blob/2755030efe66aca500bafaa893769e99a9854ef6/engine/CLAUDE.md) · 265★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Rocky

Rust SQL transformation engine. Replaces dbt's core responsibilities (DAG resolution, incremental logic, SQL generation, schema management) with a compiled, type-safe approach. No Jinja. No manifest. No parse step.

**License:** Apache 2.0

## Project Structure

Cargo workspace with 23 library crates + 2 binary crates (`rocky` + `rocky-lsp`) — 25 members total. Rust edition 2024, MSRV 1.88:

The `Plan` enum was deleted in the Phase 3 typed-IR migration; `ModelIr` is now the sole transformation intermediate, dispatched via `ModelIrVariant`. The IR data types (`ModelIr`, `ModelIrVariant`, `ProjectIr`, lakehouse format/options, column lineage, masks, time grains, `RockyType`) live in their own `rocky-ir` crate; `rocky-core` keeps the runtime surface (adapter traits, DAG executor, state store, drift, SQL generation, breaking-change classifier, ci-diff).

```
engine/                         # this directory, inside the rocky monorepo
├── Cargo.toml                  # Workspace manifest
├── crates/
│   ├── rocky-ir/               # Typed IR (data only — no runtime traits)
│   │   └── src/
│   │       ├── ir.rs           # ModelIr, ModelIrVariant, ProjectIr, MaterializationStrate
```

</details>
