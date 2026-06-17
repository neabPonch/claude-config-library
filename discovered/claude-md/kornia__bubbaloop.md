---
name: kornia__bubbaloop
source: https://github.com/kornia/bubbaloop/blob/0f57ac97f76daed25c045c61e633136342d75d56/CLAUDE.md
repo: kornia/bubbaloop
kind: claude-md
stars: 21
last_pushed: 2026-05-26T07:23:16Z
license: apache-2.0
score: 9
domains: [hardware-ai, rust, embedded-systems, iot, distributed-systems]
tags: [architecture, low-level, sdk-parity, agentic-workflow]
curated: 2026-06-16
curated_by: config-scout
---

# kornia/bubbaloop — claude-md

**Why it's worth keeping:** It establishes critical cross-language constraints (Rust/Python SDK parity) and maps specific file paths to functional roles, which is essential for preventing AI errors in complex distributed systems.

**Summary:** A high-density architectural map of a hardware orchestration system detailing file responsibilities, dataflow patterns, and communication protocols.

**Source credibility:** The technical depth suggests a high-quality, specialized engineering effort despite the lower star count.

**Recency:** Extremely current; updated within the last month.

**Source:** [kornia/bubbaloop/CLAUDE.md](https://github.com/kornia/bubbaloop/blob/0f57ac97f76daed25c045c61e633136342d75d56/CLAUDE.md) · 21★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# 🦐 Bubbaloop

Physical AI orchestration built on Zenoh. Single binary: CLI + daemon + MCP server.

## Living Documents (update these as architecture evolves)

- **ARCHITECTURE.md** — Layer model, node contract, security, open-core boundary
- **ROADMAP.md** — Implementation phases (YAML skills, agent, SQLite memory, scheduling)
- **CONTRIBUTING.md** — Agentic workflows, agent tiers, validation, two-critic loop
- **docs/concepts/dataflow.md** — Provenance envelope, manifest queryable, `bubbaloop dataflow` CLI + MCP tool (how the SDK answers "what's wired, what's flowing")

## Structure

```
crates/bubbaloop/           # Main binary (CLI + daemon + MCP server)
crates/bubbaloop-node/      # Node SDK (standalone, NOT in workspace — batteries-included framework)
crates/bubbaloop-node-build/ # Build helper for nodes (wraps prost-build, standalone)
crates/bubbaloop-schemas/   # Protobuf schemas (standalone, NOT in workspace — never add to workspace)
dashboard/                  # React + Vite + TypeScript
```

Key source files in `crates/bubbaloop/src/`:
- `cli/login.rs` — login/logout/status + `has_claude_credentials()` (env var → OAuth → key file)
- `cli/agent_setup.rs` — `bubbaloop agen
```

</details>
