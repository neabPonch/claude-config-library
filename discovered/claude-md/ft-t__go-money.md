---
name: ft-t__go-money
source: https://github.com/ft-t/go-money/blob/484e409f2dc040ec05e570b5fd0d03b2a7756231/CLAUDE.md
repo: ft-t/go-money
kind: claude-md
stars: 271
last_pushed: 2026-06-06T13:13:20Z
license: agpl-3.0
score: 10
domains: [backend-api, web-frontend, ai-agent-guidance, devops]
tags: [go, angular, mcp, fullstack, debugging-rituals]
curated: 2026-06-16
curated_by: config-scout
---

# ft-t/go-money — claude-md

**Why it's worth keeping:** It teaches the agent how to use domain-specific MCP servers for high-accuracy UI work and includes a 'Claude-in-Chrome' ritual to solve complex local development environment issues.

**Summary:** A masterclass in AI-context engineering that provides deep architectural traces, specific debugging rituals (including browser state manipulation), and project-specific MCP tool usage instructions.

**Source credibility:** High; active repository with recent commits and detailed, highly specific technical instructions.

**Recency:** Very current; utilizes Angular 19 and modern MCP server patterns.

**Source:** [ft-t/go-money/CLAUDE.md](https://github.com/ft-t/go-money/blob/484e409f2dc040ec05e570b5fd0d03b2a7756231/CLAUDE.md) · 271★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository

**Go Money** — self-hosted personal finance manager. Go backend (ConnectRPC) + Angular 19 / PrimeNG 19 frontend. PostgreSQL via GORM. Lua scripting for transaction rules. Grafana for reporting. Embedded MCP server exposed at `/mcp`.

## Layout

```
cmd/                    entrypoints (server, mcp-client, sync-exchange-rates, jwt-key-generator)
pkg/                    domain packages — each owns its interfaces.go + generated mocks
frontend/               Angular 19 SPA (PrimeNG + Tailwind)
docs/                   AI-oriented docs — start at docs/INDEX.md (schema, business-logic, mcp, analytics)
build/                  Dockerfiles + SAM for AWS exchange-rate lambda
compose/                local docker-compose stacks
helm/                   k8s chart
.mcp.json               project-scoped MCP servers (angular-cli, primeng)
```

Server wiring lives in `cmd/server/main.go` — it constructs every service with explicit deps (no DI container). Read it first to trace how a new dep threads through.

## Commands

### Go
```
make lint                            # g
```

</details>
