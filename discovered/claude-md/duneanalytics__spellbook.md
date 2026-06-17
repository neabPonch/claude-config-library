---
name: duneanalytics__spellbook
source: https://github.com/duneanalytics/spellbook/blob/85b4e891366f7433c1503290739e14c037dd2646/CLAUDE.md
repo: duneanalytics/spellbook
kind: claude-md
stars: 1498
last_pushed: 2026-06-15T15:31:00Z
license: other
score: 9
domains: [data-engineering, sql, dbt, blockchain]
tags: [monorepo, dbt, sql, devops]
curated: 2026-06-15
curated_by: config-scout
---

# duneanalytics/spellbook — claude-md

**Why it's worth keeping:** Excellent use of directory-aware command patterns essential for monorepos; defines specific custom tool patterns (`dune_query.py`) to enable Claude to inspect database state.

**Summary:** Provides structured guidance for a complex dbt monorepo used for blockchain data transformation.

**Source credibility:** High; Dune Analytics is a major industry player and the repository shows very recent activity.

**Recency:** Current; utilizes modern tooling like `uv` and provides context-rich terminal commands.

**Source:** [duneanalytics/spellbook/CLAUDE.md](https://github.com/duneanalytics/spellbook/blob/85b4e891366f7433c1503290739e14c037dd2646/CLAUDE.md) · 1498★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Spellbook is Dune Analytics' open-source interpretation layer for blockchain data. It's a **dbt monorepo** that transforms raw blockchain data into clean, usable datasets ("spells") using SQL + Jinja2 templating on DuneSQL (Trino-based).

## Repository Structure

The repo is organized as multiple independent dbt sub-projects under `dbt_subprojects/`:

- **`daily_spellbook`** — Default location for new spells (daily refresh)
- **`hourly_spellbook`** — Promoted spells with higher frequency (requires Dune team approval)
- **`dex`** — DEX and DEX aggregator trading data (includes `dex.trades`)
- **`nft`** — NFT-related models
- **`solana`** — Solana-specific models
- **`tokens`** — Token metadata, transfers, and balances

Each sub-project is self-contained with its own `dbt_project.yml`, `profiles.yml`, `models/`, `macros/`, `seeds/`, and `tests/`.

Shared resources live at the repo root:
- `sources/` — 170+ source YAML files (raw table definitions)
- `dbt_macros/` — Shared macros (`expose_spells`, `optimize_spell`, `mark_as_spell`, `enforce_join_dis
```

</details>
