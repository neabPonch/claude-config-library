---
name: davidtaing__residential_tenancy_act
source: https://github.com/davidtaing/residential_tenancy_act/blob/c05189d2558314123f548f801a5ea7588e2ecd91/CLAUDE.md
repo: davidtaing/residential_tenancy_act
kind: claude-md
stars: 0
last_pushed: 2025-08-26T00:12:30Z
license: unknown
score: 7
domains: [web-app, ai-agents, elixir]
tags: [phoenix, rag, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# davidtaing/residential_tenancy_act — claude-md

**Why it's worth keeping:** The detailed 'Data Flow' section is highly transferable; it teaches the agent how state transitions through complex RAG-based interactions across different modules.

**Summary:** Maps an Elixir/Phoenix application by defining its core domains, component responsibilities, and specific data flow paths.

**Source credibility:** Low (0 stars, solo project).

**Recency:** 10 months old; the architectural logic remains relevant regardless of tool updates.

**Source:** [davidtaing/residential_tenancy_act/CLAUDE.md](https://github.com/davidtaing/residential_tenancy_act/blob/c05189d2558314123f548f801a5ea7588e2ecd91/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

```bash
# Setup project dependencies and database
mix setup

# Start the development server
mix phx.server

# Start with IEx shell
iex -S mix phx.server

# Run tests
mix test

# Build assets
mix assets.build

# Deploy assets (minified)
mix assets.deploy

# Database operations
mix ash.setup    # Setup Ash resources and database
mix ecto.setup   # Create, migrate, and seed database
mix ecto.reset   # Drop and recreate database
```

## Architecture Overview

This is an Elixir Phoenix LiveView application that provides a chatbot interface for querying Residential Tenancy Act information. The application uses the Ash framework for resource management and authentication.

### Core Domains

- **ResidentialTenancyAct.Accounts** - User management with magic link authentication
- **ResidentialTenancyAct.Acts** - RTA sections data and similarity search functionality
- **ResidentialTenancyAct.Chat** - Chat conversations, messages, and token/prompt history

### Key Components

**LLM Integration (`lib/residential_tenancy_act/llm/`)**
- AWS Bedrock integrat
```

</details>
