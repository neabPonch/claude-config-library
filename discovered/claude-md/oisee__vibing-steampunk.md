---
name: oisee__vibing-steampunk
source: https://github.com/oisee/vibing-steampunk/blob/1989ce143851125bdd21154fab750f047f5c4151/CLAUDE.md
repo: oisee/vibing-steampunk
kind: claude-md
stars: 373
last_pushed: 2026-04-15T15:21:55Z
license: mit
score: 9
domains: [cli-tools, sap-abap, security]
tags: [mcp, go, enterprise-dev]
curated: 2026-06-15
curated_by: config-scout
---

# oisee/vibing-steampunk — claude-md

**Why it's worth keeping:** The 'Task | Files' lookup table is exceptionally efficient for agentic task routing, while the highly detailed redaction policy provides a template for maintaining security in high-stakes environments.

**Summary:** Provides an actionable mental model of the codebase through priority tracking, task-to-file mappings, and specific procedural guides. It also includes a sophisticated security protocol for sanitizing sensitive enterprise identifiers.

**Source credibility:** High; reflects deep domain expertise in SAP ABAP and structured technical documentation.

**Recency:** Very current; aligns with modern AI agent workflows.

**Source:** [oisee/vibing-steampunk/CLAUDE.md](https://github.com/oisee/vibing-steampunk/blob/1989ce143851125bdd21154fab750f047f5c4151/CLAUDE.md) · 373★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

**vsp** — Go-native MCP server and CLI for SAP ABAP Development Tools (ADT).

> **Doc intent:** CLAUDE.md = dev context. README.md = user onboarding. reports/ = research/history. contexts/ = session handoff.

---

## Current Priorities

### 1. Graph Engine (`pkg/graph/`) — In Progress
Sequence: unify existing dep logic → SQL/ADT adapters → impact/path queries.
- Done: core types, parser dep extraction, boundary analyzer (11 tests)
- Pending: SQL adapters (CROSS/WBCROSSGT/D010INC), ADT adapters, unify `cli_deps.go` + `cli_extra.go` + `ctxcomp/analyzer.go`
- Design: [002](reports/2026-04-05-002-graph-engine-design.md), [003](reports/2026-04-05-003-graph-engine-alignment-for-claude.md)

### 2. GUI Debugger (Issue #2) — Strategic
Plan: MCP debug sessions → DAP → Web UI. ADT REST API mapped from `CL_TPDA_ADT_RES_APP`. Design: [001](reports/2026-04-05-001-gui-debugger-design.md)

### 3. Open Issues
- **#88** Lock handle bug (EditSource/WriteSource) — real user report
- **#55** RunReport in APC — architectural limit
- **#46, #45** Sync script — low effort

---

## Build & Test

```bash
go build -o vsp ./cmd/vsp              # Build
go test ./...                           # Un
```

</details>
