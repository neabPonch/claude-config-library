---
name: GetBindu__Bindu
source: https://github.com/GetBindu/Bindu/blob/6ef5699a322979e550e1f344553a36ce6ebbaa22/CLAUDE.md
repo: GetBindu/Bindu
kind: claude-md
stars: 6934
last_pushed: 2026-06-08T20:38:31Z
license: other
score: 9
domains: [agents-ai, backend-api, distributed-systems]
tags: [multi-language, grpc, python, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# GetBindu/Bindu — claude-md

**Why it's worth keeping:** The 'Gotchas & What NOT to Do' section provides high-signal constraints that prevent common errors, while the ASCII architecture diagram creates a vital mental map of system dependencies.

**Summary:** A highly structured multi-language guide for a decentralized agent framework featuring Python core and TypeScript SDKs.

**Source credibility:** High; 6.9k stars and recently active/maintained repository.

**Recency:** Current; utilizes modern tooling like uv and current language standards.

**Source:** [GetBindu/Bindu/CLAUDE.md](https://github.com/GetBindu/Bindu/blob/6ef5699a322979e550e1f344553a36ce6ebbaa22/CLAUDE.md) · 6934★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project: Bindu - Decentralized Agent Framework

## Critical Context (Read First)

- **Language**: Python 3.12+ (core), TypeScript (SDK + comms UI + gateway)
- **Framework**: FastAPI/Starlette (HTTP), gRPC (cross-language), React/Vite (inbox UI)
- **Database**: MongoDB (primary), PostgreSQL (optional), Redis (caching)
- **Architecture**: Microservices with DID-based identity, OAuth2 auth, x402 payments
- **Testing**: pytest (Python), Jest (TypeScript), Playwright (E2E)

## What is Bindu?

Bindu is a framework for building **autonomous AI agents as microservices**. Each agent:
- Has a DID (Decentralized Identifier) for cryptographic identity
- Speaks the A2A (Agent-to-Agent) protocol over HTTP
- Can be written in any language via gRPC SDKs
- Supports payments via x402 protocol (USDC on Base)
- Integrates with OAuth2 (Ory Hydra) for authentication

## Commands That Work

```bash
# Python core development
uv sync                          # Install dependencies
uv run pytest                    # Run all tests
uv run pytest tests/unit         # Unit tests only
uv run pytest tests/integration  # Integration tests only
uv run ruff check .              # Lint
uv run ruff format .
```

</details>
