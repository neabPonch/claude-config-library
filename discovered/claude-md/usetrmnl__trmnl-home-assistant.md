---
name: usetrmnl__trmnl-home-assistant
source: https://github.com/usetrmnl/trmnl-home-assistant/blob/849f61d924e423e27d3b4e68de3eceb3862ffada/CLAUDE.md
repo: usetrmnl/trmnl-home-assistant
kind: claude-md
stars: 141
last_pushed: 2026-06-14T00:44:33Z
license: unknown
score: 9
domains: [backend, image-processing, iot]
tags: [architecture-diagrams, dev-workflows, environment-parity]
curated: 2026-06-15
curated_by: config-scout
---

# usetrmnl/trmnl-home-assistant — claude-md

**Why it's worth keeping:** It uses ASCII request flows, module mapping tables, and explicitly highlights critical environmental constraints (ImageMagick versioning) to prevent subtle bugs.

**Summary:** A high-density technical manual that provides deep architectural context alongside strict development workflows.

**Source credibility:** Highly professional and well-maintained repository with clear documentation standards.

**Recency:** Very current; utilizes modern toolchains like Bun 1.3.5+ and updated TypeScript configurations.

**Source:** [usetrmnl/trmnl-home-assistant/CLAUDE.md](https://github.com/usetrmnl/trmnl-home-assistant/blob/849f61d924e423e27d3b4e68de3eceb3862ffada/CLAUDE.md) · 141★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Home Assistant add-on for TRMNL e-ink displays. Captures HA dashboard screenshots with advanced dithering algorithms optimized for e-paper screens.

**Runtime:** Bun 1.3.5+ (not Node.js)
**Language:** TypeScript with strict type checking
**Image Processing:** ImageMagick 7 Q16-HDRI via `gm` package

## Development Commands

```bash
cd trmnl-ha/ha-trmnl

# Development
bun install
bun run dev                 # Hot-reload development server

# Testing
bun test                    # All tests
bun test tests/unit         # Unit tests only
bun test tests/integration  # Integration tests (requires MOCK_HA=true)
bun test --coverage         # With coverage report
bun test --watch            # Watch mode

# Run single test file
bun test tests/unit/dithering.test.ts

# Linting & Type Checking
bun run lint                # ESLint
bun run lint:fix            # Auto-fix lint issues
bun run typecheck           # TypeScript check (no emit)

# Mock HA Server (for local development without real HA)
bun run mock:server         # Start mock HA on localhost:8123
MOCK_
```

</details>
