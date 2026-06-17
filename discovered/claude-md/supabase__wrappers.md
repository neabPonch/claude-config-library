---
name: supabase__wrappers
source: https://github.com/supabase/wrappers/blob/d37f61b5faa04b69ae4ca0bfe3eacc227e83dd0a/CLAUDE.md
repo: supabase/wrappers
kind: claude-md
stars: 856
last_pushed: 2026-06-12T09:28:58Z
license: apache-2.0
score: 9
domains: [backend, database, rust]
tags: [rust, postgres, extension, fdw]
curated: 2026-06-15
curated_by: config-scout
---

# supabase/wrappers — claude-md

**Why it's worth keeping:** Provides exact trait definitions to prevent AI hallucination of interfaces; includes complete CLI workflows for building, running, and testing specialized workspaces.

**Summary:** A highly technical guide for developing Rust-based PostgreSQL extensions using the pgrx framework. It bridges the gap between documentation and implementation by providing core trait signatures and architectural context.

**Source credibility:** High; maintained by Supabase with significant community adoption (856 stars).

**Recency:** Current; uses modern Rust 1.88.0 and pgrx 0.16.1 toolchains.

**Source:** [supabase/wrappers/CLAUDE.md](https://github.com/supabase/wrappers/blob/d37f61b5faa04b69ae4ca0bfe3eacc227e83dd0a/CLAUDE.md) · 856★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - AI Assistant Guide for Wrappers

## Project Overview

Wrappers is a development framework for PostgreSQL Foreign Data Wrappers (FDWs), written in Rust. It enables querying external data sources (APIs, databases, files) as if they were regular PostgreSQL tables. The project is maintained by [Supabase](https://supabase.com).

**Documentation**: https://fdw.dev/ | **API Docs**: https://docs.rs/supabase-wrappers

## Repository Structure

```
wrappers/
├── supabase-wrappers/           # Core FDW framework library (crates.io: supabase-wrappers)
├── supabase-wrappers-macros/    # Procedural macros (#[wrappers_fdw])
├── wrappers/                    # Native FDW implementations (PostgreSQL extension)
│   └── src/fdw/                 # Individual FDW implementations
├── wasm-wrappers/               # WebAssembly-based FDW implementations (separate workspace)
│   └── fdw/                     # Individual Wasm FDW crates
└── docs/                        # MkDocs documentation site
```

## Workspace Configuration

The project uses Cargo workspaces with the following structure:

- **Main workspace** (`Cargo.toml`): Contains `supabase-wrappers`, `supabase-wrappers-macros`, and `wrap
```

</details>
