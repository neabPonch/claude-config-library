---
name: noahlh__celestite
source: https://github.com/noahlh/celestite/blob/bd5ba3af9cd6eea0f8904399e54929179a78b913/CLAUDE.md
repo: noahlh/celestite
kind: claude-md
stars: 238
last_pushed: 2026-03-20T15:55:00Z
license: mit
score: 9
domains: [web-framework, backend-api, ssr]
tags: [crystal, svelte, architecture-map]
curated: 2026-06-16
curated_by: config-scout
---

# noahlh/celestite — claude-md

**Why it's worth keeping:** The 'Request Flow' section and the breakdown of Crystal vs. Bun sides are elite; they provide the exact mental model needed to prevent errors in cross-process communication.

**Summary:** Provides a high-fidelity architectural map for a complex dual-runtime system (Crystal and Bun/Vite).

**Source credibility:** High; 238 stars indicates a useful, established tool with recent maintenance.

**Recency:** Current; highly effective for modern agentic workflows requiring multi-step execution context.

**Source:** [noahlh/celestite/CLAUDE.md](https://github.com/noahlh/celestite/blob/bd5ba3af9cd6eea0f8904399e54929179a78b913/CLAUDE.md) · 238★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Celestite is a Crystal library that enables server-side rendering (SSR) of Svelte 5 components. It spawns a Bun/Vite render server that handles SSR requests via HTTP, allowing Crystal web applications to use Svelte as their view layer.

## Commands

### Install Dependencies
```bash
shards install  # Installs Crystal deps and runs bun install via postinstall hook
```

### Run Tests
```bash
crystal spec                           # Run all tests
crystal spec spec/celestite_spec.cr    # Run specific test file
```

### Build for Production
```bash
# From svelte-scripts directory with proper env vars:
make build COMPONENT_DIR=/path/to/views BUILD_DIR=/path/to/public/celestite
```

### Development
The project is a shard (Crystal library) - no standalone run command. Tests spawn a Bun SSR server that must start within 20 seconds.

## Architecture

### Crystal Side (`src/celestite/`)
- **celestite.cr** - Main module entry point. Manages renderer lifecycle, handles SIGTERM for graceful shutdown.
- **renderer.cr** - Core SSR logic. Spawns Bun process via Ma
```

</details>
