---
name: goodhamgupta__jumpstart_ai
source: https://github.com/goodhamgupta/jumpstart_ai/blob/d7763ef8f5e6b8ee7333489b8ac3b2420dc19c96/CLAUDE.md
repo: goodhamgupta/jumpstart_ai
kind: claude-md
stars: 0
last_pushed: 2026-04-21T05:05:00Z
license: unknown
score: 8
domains: [backend-api, web-application, ai-agents]
tags: [elixir, ash-framework, phoenix, fullstack]
curated: 2026-06-16
curated_by: config-scout
---

# goodhamgupta/jumpstart_ai — claude-md

**Why it's worth keeping:** The 'Development Notes' section prescribes specific framework-specific workflows (e.g., preferring Ash commands over raw Ecto) to prevent the LLM from using generic patterns incorrectly.

**Summary:** Provides a highly structured overview of an Elixir/Ash-based AI agent application, including essential lifecycle commands and architectural boundaries.

**Source credibility:** Low social proof via stars, but demonstrates high technical maturity regarding the Elixir/Ash ecosystem.

**Recency:** Current; aligns with modern Phoenix and Ash Framework practices.

**Source:** [goodhamgupta/jumpstart_ai/CLAUDE.md](https://github.com/goodhamgupta/jumpstart_ai/blob/d7763ef8f5e6b8ee7333489b8ac3b2420dc19c96/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an AI agent application for Financial Advisors built with Elixir Phoenix and the Ash Framework. It integrates with Gmail, Google Calendar, and HubSpot to provide a ChatGPT-like interface for managing client relationships and automating tasks.

## Development Commands

- `mix setup` - Install dependencies and setup the project
- `mix phx.server` - Start the development server (runs on http://localhost:4000)
- `iex -S mix phx.server` - Start server in interactive shell
- `mix test` - Run tests (uses ash.setup --quiet before running)
- `mix ash.setup` - Setup Ash resources and run migrations
- `docker-compose up` - Start PostgreSQL database locally

### Asset Commands
- `mix assets.setup` - Install Tailwind and esbuild
- `mix assets.build` - Build assets for development
- `mix assets.deploy` - Build and minify assets for production

### Database Commands
- `mix ecto.setup` - Create database, run migrations, and seed data
- `mix ecto.reset` - Drop and recreate database with fresh data
- `mix ash.setup` - Preferred over ecto commands as it han
```

</details>
