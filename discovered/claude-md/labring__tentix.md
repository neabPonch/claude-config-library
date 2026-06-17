---
name: labring__tentix
source: https://github.com/labring/tentix/blob/424f7b1ae9cd5024793bf68280d0c4cc0883a79d/CLAUDE.md
repo: labring/tentix
kind: claude-md
stars: 404
last_pushed: 2026-06-04T10:43:50Z
license: other
score: 9
domains: [web-frontend, backend-api, monorepo]
tags: [bun, turborepo, fullstack, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# labring/tentix — claude-md

**Why it's worth keeping:** Includes high-signal sections like 'Common Gotchas' and 'Important Implementation Details' (e.g., mandatory Bun usage) that prevent LLM hallucinations during complex tasks.

**Summary:** A comprehensive guide for a Bun-based monorepo featuring detailed command sets, architectural patterns like Hono RPC, and explicit development constraints.

**Source credibility:** High; a popular open-source project with active maintenance.

**Recency:** Very current, utilizing the latest versions of React (19) and Tailwind CSS (4.0).

**Source:** [labring/tentix/CLAUDE.md](https://github.com/labring/tentix/blob/424f7b1ae9cd5024793bf68280d0c4cc0883a79d/CLAUDE.md) · 404★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Essential Commands

### Development
```bash
# Start development server (both frontend and backend)
bun run dev

# Alternative using Make
make dev

# Build the entire project
bun run build

# Run linting
bun run lint

# Run type checking
bun run typecheck

# Format code
bun run format
```

### Database Operations
```bash
cd server

# Generate database migrations
bun run generate

# Apply database migrations
bun run migrate

# Open Drizzle Studio (database GUI)
bun run studio

# Generate seed data for development
bun run seed

# Database utility scripts
bun run script/getCryptoKey.ts      # Generate encryption keys
bun run script/initDB.ts            # Initialize database with users
bun run script/resetDB.ts           # Reset database completely
bun run script/migrateStaffList.ts  # Migrate staff from Feishu
```

### Package-Specific Commands
```bash
# Frontend-specific
cd frontend
bun run dev          # Start frontend dev server
bun run build        # Build frontend
bun run test         # Run frontend tests
bun run typecheck    # Frontend type checking

# Server-sp
```

</details>
