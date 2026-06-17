---
name: evdzhurov__raft-rs
source: https://github.com/evdzhurov/raft-rs/blob/12ec76806d044b571847324247e20b1345b8fb18/CLAUDE.md
repo: evdzhurov/raft-rs
kind: claude-md
stars: 0
last_pushed: 2026-03-06T08:18:28Z
license: unknown
score: 8
domains: [systems-programming, distributed-systems]
tags: [raft, rust, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# evdzhurov/raft-rs — claude-md

**Why it's worth keeping:** The 'Known TODOs / Gaps' section is a masterclass in guiding AI through technical debt, while the architecture diagram clarifies complex module relationships.

**Summary:** Detailed structural and type-level context for an incomplete Rust consensus protocol implementation.

**Source credibility:** Single-author educational project with minimal social proof.

**Recency:** Modern; uses Rust 2024 and current async patterns.

**Source:** [evdzhurov/raft-rs/CLAUDE.md](https://github.com/evdzhurov/raft-rs/blob/12ec76806d044b571847324247e20b1345b8fb18/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# raft-rs Project Context

## Overview
Educational Raft consensus protocol implementation in Rust. Work in progress — does not yet compile.
- Rust edition: 2024
- Binary: `node` — accepts `--node-id` and `--config <json file>`

## Dependencies (Cargo.toml)
- `clap 4.5` — CLI arg parsing (derive feature)
- `log 0.4` — logging facade
- `serde 1.0` + `serde_json 1.0` — JSON serialization (cluster config)
- `tarpc 0.37` — async RPC framework (serde-transport + tcp features)

## Source Files
- `src/main.rs` — entry point: parses args, loads ClusterConfig, constructs KvStore/Node/Consensus (stubs)
- `src/messages.rs` — RPC message structs (was rpc.rs in earlier version)
- `src/rpc.rs` — tarpc service trait `RaftRpc` (async, generates client/server via `#[tarpc::service]`)
- `src/server.rs` — synchronous `Server` trait abstracting outbound RPC calls
- `src/consensus.rs` — core Raft logic
- `src/node.rs` — `Node` and `ClusterConfig`; implements both `Server` and `RaftRpc` traits
- `src/sm.rs` — `StateMachine` trait
- `src/kv.rs` — `KvStore` implementing `StateMachine`

## Key Types

### messages.rs
- `RequestVote { term, candidate_id, last_log_idx, last_log_term: i32 }`
- `RequestVoteReply
```

</details>
