---
name: highlight__highlight
source: https://github.com/highlight/highlight/blob/7a297b5fea4233d99e92177f53dada3236513616/CLAUDE.md
repo: highlight/highlight
kind: claude-md
stars: 9289
last_pushed: 2026-04-16T01:06:56Z
license: other
score: 9
domains: [backend-api, web-frontend, monorepo, observability]
tags: [monorepo, go, react, graphql, fullstack]
curated: 2026-06-15
curated_by: config-scout
---

# highlight/highlight — claude-md

**Why it's worth keeping:** Excellent breakdown of data flow and the critical mapping of 'change -> command' sequences (e.g., schema modification to codegen), which prevents agent-driven breakage.

**Summary:** A comprehensive technical blueprint for a complex monorepo that links commands to architectural patterns.

**Source credibility:** High; based on a highly-starred, actively maintained observability platform.

**Recency:** Very current, utilizing modern tech stacks like Go 1.23 and React 18/Vite.

**Source:** [highlight/highlight/CLAUDE.md](https://github.com/highlight/highlight/blob/7a297b5fea4233d99e92177f53dada3236513616/CLAUDE.md) · 9289★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is Highlight.io, a full-stack observability platform that provides session replay, error monitoring, logging, and distributed tracing capabilities. The repository is structured as a monorepo containing:

- **Backend**: Go-based GraphQL API server with dual public/private GraphQL endpoints
- **Frontend**: React/TypeScript dashboard application built with Vite
- **SDKs**: Multi-language client libraries for integrating with Highlight
- **RRWeb**: Forked session replay recording library (submodule)
- **Infrastructure**: Docker compose and deployment configurations

## Key Development Commands

### Backend Development
```bash
# In /backend directory
make start            # Start backend with doppler (recommended)
make start-no-doppler # Start backend without doppler
make debug            # Start with debugger attached
make test             # Run all tests with race detection
make migrate          # Run database migrations
make public-gen       # Generate public GraphQL schema
make private-gen      # Generate private GraphQL schema
```

### Fr
```

</details>
