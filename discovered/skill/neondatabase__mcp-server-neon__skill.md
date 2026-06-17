---
name: neondatabase__mcp-server-neon__skill
source: https://github.com/neondatabase/mcp-server-neon/blob/67834e659e1df3d78317d4dc85aee7390d4214b0/.agents/skills/claimable-postgres/SKILL.md
repo: neondatabase/mcp-server-neon
kind: skill
stars: 609
last_pushed: 2026-06-05T17:36:06Z
license: mit
score: 9
domains: [backend, database, devops, cli-tools]
tags: [postgres, neon, provisioning, development]
curated: 2026-06-15
curated_by: config-scout
---

# neondatabase/mcp-server-neon — skill

**Why it's worth keeping:** The 'Agent Workflow' section provides a perfect template for stateful tasks, moving from intent confirmation through execution to verification and user notification.

**Summary:** Enables an agent to provision instant, temporary Postgres databases using the 'npx get-db' utility for rapid prototyping.

**Source credibility:** High; Neon is a major industry player in serverless Postgres with an actively maintained repository.

**Recency:** Very recent; the instructions align perfectly with modern CLI-driven development workflows used by Claude Code.

**Source:** [neondatabase/mcp-server-neon/.agents/skills/claimable-postgres/SKILL.md](https://github.com/neondatabase/mcp-server-neon/blob/67834e659e1df3d78317d4dc85aee7390d4214b0/.agents/skills/claimable-postgres/SKILL.md) · 609★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: claimable-postgres
description: >-
  Provision instant temporary Postgres databases via Claimable Postgres by Neon
  (pg.new) with no login, signup, or credit card. Use when users ask for a
  quick Postgres environment, a throwaway DATABASE_URL for prototyping/tests,
  or "just give me a DB now". Triggers include: "quick postgres", "temporary
  postgres", "no signup database", "no credit card database", "instant
  DATABASE_URL".
---

# Claimable Postgres

Create an instant Postgres database with Claimable Postgres by Neon (`pg.new`) for fast local development, demos, prototyping, and test environments.

Databases are temporary by default (typically 72 hours) and can be claimed later to a Neon account for permanent use.

## Quick Start

Run:

```bash
npx get-db
```

This provisions a database and writes `DATABASE_URL` to `.env`.

## When to Use Which Method

### CLI (`npx get-db`)

Use this by default for most users who want a fast setup in an existing project.

```bash
npx get-db
```

Common flags:

- `-y, --yes`: skip prompts
- `-e, --env <path>`: choose env file path
- `-k, --key <name>`: customize env var key (default `DATABASE_URL`)
- `-s, --seed <path>`: run SQL seed
```

</details>
