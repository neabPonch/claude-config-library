---
name: cxmbill97__AI_DM
source: https://github.com/cxmbill97/AI_DM/blob/29305032749bbf22815dd403b1cf5331856683ed/claude.md
repo: cxmbill97/AI_DM
kind: claude-md
stars: 1
last_pushed: 2026-04-16T05:53:10Z
license: unknown
score: 9
domains: [backend-api, agents-ai, fullstack]
tags: [multi-agent, annotated-tree, operational-manual]
curated: 2026-06-15
curated_by: config-scout
---

# cxmbill97/AI_DM — claude-md

**Why it's worth keeping:** The inclusion of 'Core Principles' (e.g., Deterministic State > LLM Output) provides essential behavioral guidance, while the annotated file tree maps logic to location more effectively than a standard README.

**Summary:** Provides a high-density operational manual containing specific command patterns and a functionally annotated directory tree.

**Source credibility:** Low-star personal project, but demonstrates professional-grade documentation depth.

**Recency:** Very recent; utilizes modern tooling like 'uv' and MCP servers.

**Source:** [cxmbill97/AI_DM/claude.md](https://github.com/cxmbill97/AI_DM/blob/29305032749bbf22815dd403b1cf5331856683ed/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Commands

```bash
cd backend && uv run uvicorn app.main:app --reload --host 0.0.0.0   # API (port 8000)
cd backend && uv run pytest tests/ -x -v                             # all tests
cd backend && uv run pytest tests/ -x -v --ignore=tests/test_eval.py # skip slow LLM tests
cd backend && uv run python -m eval --scenarios all                  # eval harness
cd backend && uv run python -m mcp_server                            # MCP server (stdio)
cd frontend && pnpm dev --host 0.0.0.0                               # UI (port 5173)
./start.sh                                                            # one-command startup
```

## Project Overview

AI-powered game master for multiplayer social deduction games: Turtle Soup (海龟汤)
and Murder Mystery (剧本杀). Bilingual (zh/en). Multi-agent architecture with
minimum-privilege context isolation.

**Completed phases:**

- Phase 1: Single-player turtle soup
- Phase 2: Multiplayer + clue system + DM intervention
- Phase 3: VisibilityRegistry + per-player private clues
- Phase 4: 剧本杀 + multi-agent pipeline + voting + NPC
- Phase 5: Bilingual (zh/en) + LAN access
- Phase 6: Remote access (ngrok/cloudflare) + demo packaging + 3-play
```

</details>
