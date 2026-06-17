---
name: gsmlg-dev__phoenix_socket_client
source: https://github.com/gsmlg-dev/phoenix_socket_client/blob/abc2888a4297ca109cf0f48ee64b3fbefa15800e/CLAUDE.md
repo: gsmlg-dev/phoenix_socket_client
kind: claude-md
stars: 0
last_pushed: 2026-03-15T15:31:47Z
license: mit
score: 9
domains: [elixir, realtime-communication]
tags: [supervision-tree, elixir, websocket]
curated: 2026-06-15
curated_by: config-scout
---

# gsmlg-dev/phoenix_socket_client — claude-md

**Why it's worth keeping:** The text-based architecture diagram provides critical high-level context on process hierarchies. It also includes precise, granular test execution patterns.

**Summary:** Provides comprehensive development commands and a structural overview of the system's supervision tree.

**Source credibility:** Low star count but demonstrates professional documentation standards for an Elixir library.

**Recency:** Highly relevant; reflects modern Elixir and Claude Code best practices.

**Source:** [gsmlg-dev/phoenix_socket_client/CLAUDE.md](https://github.com/gsmlg-dev/phoenix_socket_client/blob/abc2888a4297ca109cf0f48ee64b3fbefa15800e/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview
Elixir Phoenix Channels client library for establishing WebSocket connections and managing channel subscriptions.

## Development Commands
```bash
# Setup
mix deps.get          # Install dependencies
mix compile          # Compile the project

# Development workflow
mix format           # Format code
mix test             # Run all tests
mix test --cover     # Run tests with coverage
mix test test/file/name_test.exs:line  # Run specific test
mix test path/to/file_test.exs          # Run specific test file
mix clean            # Clean compiled files

# Quality checks
mix format --check-formatted
mix compile --warnings-as-errors
mix lint                         # credo --strict + dialyzer
```

## Architecture

Supervision tree per socket instance:
```
Phoenix.SocketClient (API wrapper, starts Supervisor)
└── Phoenix.SocketClient.Supervisor
    ├── Phoenix.SocketClient.Agent (process-scoped state storage)
    ├── Phoenix.SocketClient.Socket (GenServer - WebSocket connection lifecycle)
    └── Phoenix.SocketClient.ChannelManager (DynamicSupervisor)
```

</details>
