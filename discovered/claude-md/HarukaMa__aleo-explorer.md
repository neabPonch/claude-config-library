---
name: HarukaMa__aleo-explorer
source: https://github.com/HarukaMa/aleo-explorer/blob/901a2b3cbfdb5c956e0b236213d7a3157a192940/CLAUDE.md
repo: HarukaMa/aleo-explorer
kind: claude-md
stars: 131
last_pushed: 2026-06-02T22:42:21Z
license: agpl-3.0
score: 9
domains: [blockchain, backend, python]
tags: [asyncio, architecture-documentation, systems-programming]
curated: 2026-06-14
curated_by: config-scout
---

# HarukaMa/aleo-explorer — claude-md

**Why it's worth keeping:** It proactively suppresses common LLM 'corrections' (like star imports) and includes critical environmental warnings regarding Python CPython bugs/toolchain requirements.

**Summary:** A highly detailed guide that explains complex multi-component architecture and specific technical nuances of a blockchain explorer.

**Source credibility:** High; the repository is active, well-starred, and provides specific technical depth typical of mature open-source projects.

**Recency:** Current; utilizes modern tooling like `uv` and specific Rust toolchain versions.

**Source:** [HarukaMa/aleo-explorer/CLAUDE.md](https://github.com/HarukaMa/aleo-explorer/blob/901a2b3cbfdb5c956e0b236213d7a3157a192940/CLAUDE.md) · 131★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Aleo Explorer — an open-source blockchain explorer for the Aleo network. It runs a non-validating light node that connects to a trusted peer to fetch and index blockchain data into PostgreSQL. The active branch is `mainnet-newdb` (Postgres-only, no Redis).

## Build & Run Commands

```bash
# Install dependencies (requires Rust 1.81+ toolchain for aleo-explorer-rust)
uv sync

# Run the explorer
uv run python -m main

# Lint
uv run ruff check src/

# Type check (strict mode configured in pyproject.toml)
pyright

# Docker
docker-compose up -d
```

There are no tests in this repository.

## Configuration

Environment variables via `.env` file (see `.env.example`). Key vars:
- `DB_HOST`, `DB_USER`, `DB_PASS`, `DB_DATABASE`, `DB_SCHEMA` — PostgreSQL connection
- `P2P_NODE_HOST`, `P2P_NODE_PORT` — trusted Aleo node to sync from
- `HOST`/`PORT` — webui server (default 127.0.0.1:8000)
- `API_HOST`/`API_PORT` — API server
- `DEV_MODE=1` — uses dev genesis block
- `NETWORK` — network name (mainnet/testnet/canary)

Database schema is initialized from `pg_dum
```

</details>
