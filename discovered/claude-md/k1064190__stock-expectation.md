---
name: k1064190__stock-expectation
source: https://github.com/k1064190/stock-expectation/blob/1d07dd33ab95361a26adbe99d84c941928be979d/CLAUDE.md
repo: k1064190/stock-expectation
kind: claude-md
stars: 1
last_pushed: 2026-06-04T07:21:29Z
license: unknown
score: 9
domains: [cli-tools, agents-ai, finance]
tags: [command-patterns, skill-registry, uv-environment]
curated: 2026-06-15
curated_by: config-scout
---

# k1064190/stock-expectation — claude-md

**Why it's worth keeping:** Provides exhaustive 'command-line' templates that allow an agent to interact with the project without guessing syntax; categorizes 'skills' into functional groups for better task planning.

**Summary:** Highly detailed documentation of system architecture, CLI command patterns, and a categorized registry of specialized AI skills.

**Source credibility:** Detailed, highly structured technical documentation despite low repository star count.

**Recency:** Extremely current; uses modern tooling like `uv` and structured skill management patterns.

**Source:** [k1064190/stock-expectation/CLAUDE.md](https://github.com/k1064190/stock-expectation/blob/1d07dd33ab95361a26adbe99d84c941928be979d/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Stock Expectation

Stock prediction system with track record for US and Korean markets.

> **Status:** The `/expect` redesign was merged into `master` via [PR #2](https://github.com/k1064190/stock-expectation/pull/2)
> on 2026-05-11 (squash commit `d2ef519`). For full background on the staged work — stage outcomes, test inventory,
> code-review history, known issues, operator runbook, and pending decision points — read
> [`docs/HANDOFF.md`](docs/HANDOFF.md). The live-E2E follow-up patches are documented in
> [`docs/stage-4.1/e2e-followups.md`](docs/stage-4.1/e2e-followups.md). Remaining decision points
> (Stage 7-A/7-B live verification, PyKRX xfail, skill catalog second pass) are in HANDOFF.md §11.

## Architecture

CLI-first with `bin/stock-cli` + Claude Code skills + lightweight Python scheduler:
- `stock_cli.py` — single CLI entry point with all subcommands
- `bin/stock-cli` — bash wrapper that runs stock-cli via `uv run`
- `mcp-market-data/providers/` — US and KR market data providers (name kept for legacy reasons)
- `mcp-prediction-store/` — Prediction schema, DB CRUD, metrics computation
- `portfolio/` — Manual portfolio tracking, trade recording, evaluation
- `.claude/ski
```

</details>
