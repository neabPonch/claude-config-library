---
name: moreal__agilestory.blog
source: https://github.com/moreal/agilestory.blog/blob/de8fa513e197e068d1f3246998a279eaee556e18/CLAUDE.md
repo: moreal/agilestory.blog
kind: claude-md
stars: 8
last_pushed: 2025-12-05T06:45:45Z
license: agpl-3.0
score: 8
domains: [web-development, data-processing]
tags: [deno, astro, architecture-patterns]
curated: 2026-06-16
curated_by: config-scout
---

# moreal/agilestory.blog — claude-md

**Why it's worth keeping:** The inclusion of a visual data flow diagram and explicit design pattern descriptions (e.g., Fallback Chain) is a top-tier technique for helping AI understand system intent. The specific testing constraints further ensure high-quality, predictable code generation.

**Summary:** Provides comprehensive development commands, detailed architectural layering, and specific coding standards for a Deno/Astro application.

**Source credibility:** Small project with highly structured, professional-grade technical documentation.

**Recency:** Current; uses modern Deno and Astro patterns compatible with today's development workflows.

**Source:** [moreal/agilestory.blog/CLAUDE.md](https://github.com/moreal/agilestory.blog/blob/de8fa513e197e068d1f3246998a279eaee556e18/CLAUDE.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with
code in this repository.

## Development Commands

### Web Development

```bash
# Start development server with file watching
deno task web:dev

# Build the application
deno task web:build

# Preview production build
deno task web:preview

# Lint, format, and type check
deno task web:check
```

### Data Management

```bash
# Download content from Internet Archive (requires AGILEDATA env var)
AGILEDATA=/path/to/store deno task tool:download

# Dump processed data to JSON file
AGILEDATA=/path/to/store deno task tool:dump-file data.json
```

### Testing

```bash
# Run all tests
deno test

# Run specific test file
deno test repositories/content/persistent.test.ts

# Run tests with coverage
deno test --coverage
```

## Architecture Overview

This is an **Astro framework** application that archives and serves blog content
from Internet Archive's Wayback Machine. The architecture follows **Clean
Architecture principles** with clear separation of concerns.

### Core Architecture Layers

**Models** (`models/`): Zod-based validation schemas for `Content` and `TimeMap`
entities with runtime type safety.
```

</details>
