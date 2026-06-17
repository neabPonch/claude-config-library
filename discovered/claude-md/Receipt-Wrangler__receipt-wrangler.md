---
name: Receipt-Wrangler__receipt-wrangler
source: https://github.com/Receipt-Wrangler/receipt-wrangler/blob/53af2491a5f3ef093e13738d225e805702afb493/CLAUDE.md
repo: Receipt-Wrangler/receipt-wrangler
kind: claude-md
stars: 229
last_pushed: 2026-06-15T13:24:44Z
license: unknown
score: 9
domains: [monorepo, fullstack, api-driven]
tags: [monorepo, api-generation, workflow-automation, polyglot]
curated: 2026-06-15
curated_by: config-scout
---

# Receipt-Wrangler/receipt-wrangler — claude-md

**Why it's worth keeping:** It emphasizes 'Single Source of Truth' workflows with explicit regeneration commands and includes a high-value 'Common Pitfalls' section to prevent AI-driven errors.

**Summary:** This config provides a comprehensive architectural map for a polyglot monorepo. It bridges the gap between backend API changes and frontend/mobile client synchronization.

**Source credibility:** Solid; comes from a well-maintained, specialized full-stack application.

**Recency:** Very current; uses modern versions like Go 1.24 and Angular 19.

**Source:** [Receipt-Wrangler/receipt-wrangler/CLAUDE.md](https://github.com/Receipt-Wrangler/receipt-wrangler/blob/53af2491a5f3ef093e13738d225e805702afb493/CLAUDE.md) · 229★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Receipt Wrangler is a full-stack receipt management and splitting application with OCR-powered scanning, AI-assisted data extraction, and multi-user group management. This is a **monorepo** containing three main components:

- **api/** - Go backend service (port 8081)
- **desktop/** - Angular 19 web interface (port 4200 dev, port 80 production)
- **mobile/** - Flutter cross-platform mobile app
- **docker/** - Monolith Docker build configuration

Each component has its own CLAUDE.md with detailed component-specific guidance. This file covers monorepo-level architecture and workflows.

## Monorepo Architecture

### Component Communication
- **API Contract**: OpenAPI 3.1 specification in `api/swagger.yml` defines the API contract
- **Client Generation**: API clients are auto-generated from swagger.yml using `api/generate-client.sh`
  - Desktop: TypeScript Angular client → `desktop/src/open-api/`
  - Mobile: Dart Dio client → `mobile/api/`
  - MCP: TypeScript client for MCP integration
- **Development Flow**: Changes to API → update swagger.yml → reg
```

</details>
