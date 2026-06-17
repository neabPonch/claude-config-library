---
name: ClaperCo__Claper
source: https://github.com/ClaperCo/Claper/blob/7db48f592f8a12454308d2bc6f99f8cf01cf2fec/CLAUDE.md
repo: ClaperCo/Claper
kind: claude-md
stars: 758
last_pushed: 2026-06-14T13:44:38Z
license: agpl-3.0
score: 9
domains: [web-app, elixir-phoenix, real-time]
tags: [phoenix, elixir, liveview, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# ClaperCo/Claper — claude-md

**Why it's worth keeping:** It maps specific business domains to their respective code locations and explains high-level patterns like PubSub vs. LiveView usage, which provides vital context for an AI agent.

**Summary:** Provides essential development commands and a structured architectural overview of a Phoenix/Elixir application.

**Source credibility:** High; comes from a popular (758 stars) and actively maintained repository.

**Recency:** Current; reflects modern Phoenix/LiveView development workflows.

**Source:** [ClaperCo/Claper/CLAUDE.md](https://github.com/ClaperCo/Claper/blob/7db48f592f8a12454308d2bc6f99f8cf01cf2fec/CLAUDE.md) · 758★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Common Development Commands

### Setup and Dependencies
```bash
# Install dependencies
mix deps.get
mix setup  # Runs deps.get + ecto.setup

# Setup database
mix ecto.setup  # Creates DB, runs migrations, seeds
mix ecto.reset  # Drops DB and runs ecto.setup

# Install frontend dependencies
cd assets && npm install && cd ..
```

### Running the Application
```bash
# Start Phoenix server
mix phx.server

# Or inside IEx
iex -S mix phx.server
```

### Testing
```bash
# Run tests
mix test

# Run specific test file
mix test test/path/to/test_file.exs

# Run test with specific line number
mix test test/path/to/test_file.exs:42
```

### Code Quality
```bash
# Format code
mix format

# Run Credo for code analysis
mix credo
```

### Building Assets
```bash
# For production deployment
mix assets.deploy
```

## High-Level Architecture

Claper is an interactive presentation platform built with Phoenix Framework and Elixir. It enables real-time audience interaction during presentations through polls, forms, messages, and quizzes.

### Core Components

1. **Phoenix LiveView Arch
```

</details>
