---
name: devendranl__sapien__sapien-claude
source: https://github.com/devendranl/sapien/blob/5807d3c11ae4cc1d9a0d9e249c70dd9ce578d4bc/docs/sapien-CLAUDE.md.md
repo: devendranl/sapien
kind: claude-md
stars: 0
last_pushed: 2026-02-23T05:01:48Z
license: unknown
score: 9
domains: [backend-api, monorepo, systems-architecture]
tags: [simulation-first, microservices, enterprise, typescript]
curated: 2026-06-16
curated_by: config-scout
---

# devendranl/sapien — claude-md

**Why it's worth keeping:** The 'Simulation-First' principle is a brilliant pattern for preventing AI dependency issues, while the granular repository tree provides essential spatial awareness for large monorepos.

**Summary:** Establishes a 'simulation-first' architecture where all external dependencies must have mock implementations to ensure development remains autonomous and stable. It serves as a high-level architectural blueprint rather than just a list of commands.

**Source credibility:** Low social proof (0 stars), but reflects high professional architectural maturity.

**Recency:** Very recent; uses current toolchains like Node 20 and TypeScript 5.

**Source:** [devendranl/sapien/docs/sapien-CLAUDE.md.md](https://github.com/devendranl/sapien/blob/5807d3c11ae4cc1d9a0d9e249c70dd9ce578d4bc/docs/sapien-CLAUDE.md.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Sapien: Internet Provisioning System

> This file is the single source of truth for all Claude Code CLI sessions working on Sapien.
> Read this ENTIRE file before making any changes to the codebase.

## Project Identity

- **Name:** Sapien
- **Type:** Enterprise Internet Provisioning System for Telecom/ISP operators
- **Architecture:** Simulation-first, API-first, event-driven microservices
- **Solo Developer:** Devendra (founder-CTO)
- **AI Development Model:** Autonomous Claude Code CLI sessions — one agent, one service, one branch

## Core Design Principle: Simulation-First

**CRITICAL — READ THIS BEFORE WRITING ANY CODE:**

Sapien is designed to operate within a fully simulated ecosystem before any live system integration. Every integration boundary — northbound (toward BSS/portals/customers) and southbound (toward network/OSS/infrastructure) — MUST have a corresponding mock implementation.

This means:
- Every external adapter MUST implement a common interface with two implementations: `RealAdapter` and `MockAdapter`
- Adapter selection is controlled via environment configuration (`SAPIEN_MODE=simulation | production`)
- The mock data engine is a first-class serv
```

</details>
