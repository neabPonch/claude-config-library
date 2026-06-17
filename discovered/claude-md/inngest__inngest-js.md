---
name: inngest__inngest-js
source: https://github.com/inngest/inngest-js/blob/db89151ae6e26b107db70b9e41636daf20509729/CLAUDE.md
repo: inngest/inngest-js
kind: claude-md
stars: 966
last_pushed: 2026-06-12T23:31:09Z
license: gpl-3.0
score: 9
domains: [backend, sdk, monorepo, typescript]
tags: [monorepo-guide, testing-strategies, coding-patterns, toolchain-constraints]
curated: 2026-06-14
curated_by: config-scout
---

# inngest/inngest-js — claude-md

**Why it's worth keeping:** Includes practical 'Good vs Bad' code patterns for logging and explicitly defines the multi-layered testing strategy necessary for an SDK.

**Summary:** Provides comprehensive context for a complex monorepo SDK, including specific command execution paths and testing tiers.

**Source credibility:** High; Inngest is a highly-starred, actively maintained developer tool.

**Recency:** 

**Source:** [inngest/inngest-js/CLAUDE.md](https://github.com/inngest/inngest-js/blob/db89151ae6e26b107db70b9e41636daf20509729/CLAUDE.md) · 966★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Agent Guidance

This file provides guidance to AI coding agents when working with code in this repository.

## Repository Overview

This is the official Inngest JavaScript/TypeScript SDK - a monorepo containing packages for building serverless event-driven systems, background jobs, and durable step functions. The SDK provides framework adapters for Next.js, Express, SvelteKit, and 15+ other frameworks.

## Development Workflow

### Setup
```bash
# Use pnpm (required, enforced by preinstall hook)
cd packages/inngest/
pnpm dev  # Installs deps, builds, lints, and watches for changes
```

### Common Commands

**Main development (in `packages/inngest/`):**
```bash
pnpm dev              # Watch mode: builds + lints on changes
pnpm test             # Run unit tests
pnpm test --watch     # Watch mode testing
pnpm build            # Build the package
pnpm lint             # Run Biome linting
pnpm local:pack       # Create inngest.tgz for local testing
pnpm dev:example      # Test with example projects
pnpm itest <example>  # Run integration tests against examples
```

**Root level commands:**
```bash
pnpm build            # Build all packages recursively
```

### Testing Strategy

1. **U
```

</details>
