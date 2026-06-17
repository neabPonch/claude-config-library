---
name: guarzo__eveDMV
source: https://github.com/guarzo/eveDMV/blob/92fd384495ae73be08d35fc961db38bff8b99797/CLAUDE.md
repo: guarzo/eveDMV
kind: claude-md
stars: 0
last_pushed: 2026-05-06T03:11:19Z
license: unknown
score: 9
domains: [backend, elixir-phoenix, data-pipeline]
tags: [ash-framework, database-partitioning, clean-code-rules, elixir]
curated: 2026-06-15
curated_by: config-scout
---

# guarzo/eveDMV — claude-md

**Why it's worth keeping:** The 'Critical Development Rules' section is a masterclass in preventing AI laziness by explicitly banning placeholders and magic numbers. The specific instructions on environment-specific database configuration (pg_cron vs. SQL Sandbox) are also excellent for reducing setup errors.

**Summary:** A highly detailed technical manual for an Elixir/Ash Framework project that covers complex database partitioning and real-time pipelines.

**Source credibility:** Low social proof (0 stars), but the technical depth suggests high-quality, expert documentation.

**Recency:** Very current; references modern versions like Elixir 1.19 and Phoenix 1.8.

**Source:** [guarzo/eveDMV/CLAUDE.md](https://github.com/guarzo/eveDMV/blob/92fd384495ae73be08d35fc961db38bff8b99797/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

EVE DMV is an Elixir Phoenix application for real-time PvP intelligence and analytics for EVE Online. It uses:
- **Phoenix 1.8** with LiveView for real-time UI updates
- **Ash Framework 3.7** for declarative resource management (replaces traditional Ecto schemas)
- **Broadway** for high-throughput killmail ingestion pipeline
- **PostgreSQL 18** with partitioning and materialized views for performance
- **EVE SSO OAuth2** for authentication with automatic token refresh
- **OpenTelemetry** for observability and performance monitoring
- **Elixir 1.19** (required version)

## Essential Commands

```bash
# Setup and Development
mix setup              # Full setup: deps, DB, migrations, assets
mix phx.server         # Start Phoenix server (http://localhost:4010)
iex -S mix phx.server  # Start with interactive shell

# Database Operations
mix ecto.create        # Create database
mix ecto.migrate       # Run migrations
mix ecto.rollback      # Rollback migration
mix ecto.reset         # Drop, create, and migrate

# Testing and Quality
mix test
```

</details>
