---
name: gsmlg-dev__phoenix-react
source: https://github.com/gsmlg-dev/phoenix-react/blob/1b4d54191fba3c827bb56f6e66c1fd9a701bc4bd/CLAUDE.md
repo: gsmlg-dev/phoenix-react
kind: claude-md
stars: 52
last_pushed: 2026-03-06T08:33:48Z
license: mit
score: 9
domains: [elixir, web-frameworks, ssr]
tags: [phoenix, react, server-side-rendering, bun, deno]
curated: 2026-06-15
curated_by: config-scout
---

# gsmlg-dev/phoenix-react — claude-md

**Why it's worth keeping:** Includes critical technical nuances like file extensions required by different runtimes and provides concrete code examples for configuration and usage patterns.

**Summary:** Details a complex Phoenix/React SSR integration, covering dual runtime support (Bun/Deno) and specific architectural layers.

**Source credibility:** Decent star count for a niche tool; reflects high-quality documentation of an integration layer.

**Recency:** Current, reflecting modern Elixir/Phoenix and JS runtime workflows.

**Source:** [gsmlg-dev/phoenix-react/CLAUDE.md](https://github.com/gsmlg-dev/phoenix-react/blob/1b4d54191fba3c827bb56f6e66c1fd9a701bc4bd/CLAUDE.md) · 52★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Phoenix.ReactServer** is a Phoenix framework package that enables server-side rendering of React components within Phoenix HTML templates. It provides a rendering server that can render React components to static markup, strings, or readable streams, with support for client-side hydration.

## Architecture

The system consists of three main layers:

1. **Elixir Layer**: Phoenix integration components
2. **Runtime Layer**: JavaScript runtime servers (Bun or Deno)
3. **Client Layer**: JavaScript hydration and LiveView integration

### Core Components

- `Phoenix.ReactServer` - Main supervisor and public API
- `Phoenix.ReactServer.Server` - GenServer that manages rendering requests and caching
- `Phoenix.ReactServer.Runtime` - Dynamic supervisor for runtime processes
- `Phoenix.ReactServer.Runtime.Bun` - Bun-based runtime implementation with hot reloading
- `Phoenix.ReactServer.Runtime.Deno` - Deno-based runtime implementation with enhanced security
- `Phoenix.ReactServer.Cache` - ETS-based caching layer with TTL support
- `Phoenix.ReactServer.Hel
```

</details>
