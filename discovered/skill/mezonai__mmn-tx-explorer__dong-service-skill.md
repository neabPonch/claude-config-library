---
name: mezonai__mmn-tx-explorer__dong-service-skill
source: https://github.com/mezonai/mmn-tx-explorer/blob/d92607fbb93d0b9e5baa70199b38f78e747d4cf9/.opencode/dong-service-skill.md
repo: mezonai/mmn-tx-explorer
kind: skill
stars: 5
last_pushed: 2026-05-19T07:45:23Z
license: unknown
score: 8
domains: [backend-api, go-lang, blockchain]
tags: [backend, go, api-service, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# mezonai/mmn-tx-explorer — skill

**Why it's worth keeping:** The 'Commands' and 'Verification' sections provide explicit instructions that prevent agent hallucination during task execution. The 'Working Notes' section provides crucial domain-specific guardrails regarding numerical precision.

**Summary:** A highly actionable service skill file for a Go/PostgreSQL backend. It maps the directory structure, command-line workflows, and critical verification steps.

**Source credibility:** High; based on a functional, actively maintained blockchain service repository.

**Recency:** Current; follows modern Go development and documentation standards compatible with current AI agents.

**Source:** [mezonai/mmn-tx-explorer/.opencode/dong-service-skill.md](https://github.com/mezonai/mmn-tx-explorer/blob/d92607fbb93d0b9e5baa70199b38f78e747d4cf9/.opencode/dong-service-skill.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Dong Service Skill

## Overview
Main backend service handling core features: donation campaigns, lucky money (lì xì), P2P trading, and wallet management.

## Tech Stack
- Go 1.25 with Gin framework
- PostgreSQL
- Redis for JWT token whitelist
- JWT authentication with OAuth2
- ZK (Zero-Knowledge) proof verification
- golangci-lint for linting

## Directory Structure
```
dong-service/
├── config/        # Configuration (Viper)
├── database/      # PostgreSQL and Redis connections
├── handlers/      # HTTP request handlers
├── middleware/    # Auth, CORS, rate limiting, ZK auth
├── models/       # Data models
├── repository/    # Data access layer
├── routes/       # API route definitions
├── services/     # Business logic
├── scheduler/    # Background jobs
├── constants/    # Constants (errors, event types, status, multipliers)
├── types/        # Custom types (BigInt string handling)
├── utils/        # Helpers (amount, crypto, json, etc.)
├── logger/       # Logging (zerolog + lumberjack)
├── blockchain/   # Blockchain integration
├── migrations/   # SQL migrations (001-028)
└── docs/         # Swagger documentation
```

## Commands
```bash
cd dong-service

# Using Makefile
mak
```

</details>
