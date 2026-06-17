---
name: Ataraxy-Labs__inspect
source: https://github.com/Ataraxy-Labs/inspect/blob/90a8a5dd3a15c39e59062e2518171615fecff5c3/SKILL.md
repo: Ataraxy-Labs/inspect
kind: skill
stars: 174
last_pushed: 2026-05-22T04:44:07Z
license: other
score: 8
domains: [cli-tools, agents-ai, devops, security]
tags: [risk-assessment, mcp, code-review, dependency-analysis]
curated: 2026-06-14
curated_by: config-scout
---

# Ataraxy-Labs/inspect — skill

**Why it's worth keeping:** The strategy of reducing token volume through structural triage (calculating blast radius/dependency depth) is a top-tier pattern for agentic workflows. It transforms raw diffs into semantic, high-risk clusters that provide better context than standard linear line-by-line reading.

**Summary:** Implements risk-based triage by analyzing entity dependency graphs to prioritize high-impact changes for LLM review.

**Source credibility:** High; the project demonstrates significant technical complexity with a Rust-based analysis engine and dedicated MCP server implementation.

**Recency:** Current; actively maintained with modern tech stack components like Next.js 15.

**Source:** [Ataraxy-Labs/inspect/SKILL.md](https://github.com/Ataraxy-Labs/inspect/blob/90a8a5dd3a15c39e59062e2518171615fecff5c3/SKILL.md) · 174★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# inspect

Entity-level code review for Git. Scores changes by risk and groups them by logical dependency.

## Structure

Cargo workspace at repo root:
- `inspect-core` — analysis engine, LLM integration, risk scoring
- `inspect-cli` — CLI (`inspect diff`, `inspect pr`, `inspect review`, `inspect predict`)
- `inspect-mcp` — MCP server (6 tools)
- `inspect-api` — REST API (Axum, JWT auth, deployed via Docker)

Separate Next.js website in `docs/` (deployed to inspect.ataraxy-labs.com via Vercel "site" project).

## Build & Test

```bash
cargo build --release -p inspect-cli     # binary at target/release/inspect
cargo build --release -p inspect-mcp     # binary at target/release/inspect-mcp
cargo test --workspace                   # 12 tests
```

## Key Paths

- Risk scoring: `crates/inspect-core/src/`
- CLI commands: `crates/inspect-cli/src/commands/`
- MCP tools: `crates/inspect-mcp/src/`
- API routes: `crates/inspect-api/src/`
- Website: `docs/` (Next.js 15, Clerk auth, Supabase, Stripe billing)
- Benchmarks: `benchmarks/`

## Website (docs/)

The `docs/` directory is the live website. Vercel project name is "site" (root dir set to `docs/`).
- Auth: Clerk
- DB: Supabase
- Billing:
```

</details>
