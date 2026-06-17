---
name: cryfs__cryfs-web-next
source: https://github.com/cryfs/cryfs-web-next/blob/fd4b5ce3625a418ea30f3ea0b3e936557476f4ba/CLAUDE.md
repo: cryfs/cryfs-web-next
kind: claude-md
stars: 0
last_pushed: 2026-04-13T22:48:37Z
license: unknown
score: 7
domains: [monorepo, web-frontend, backend-api]
tags: [monorepo, delegation, context-management]
curated: 2026-06-16
curated_by: config-scout
---

# cryfs/cryfs-web-next — claude-md

**Why it's worth keeping:** Demonstrates the 'delegation pattern' where the root file points the agent to specialized sub-directory CLAUDE.md files, preventing context bloat.

**Summary:** Acts as a high-level orchestrator for a monorepo by defining structure and delegating task-specific guidance.

**Source credibility:** Low star count, but indicates a well-structured professional monorepo setup.

**Recency:** Highly current; specifically designed for modern multi-package project structures.

**Source:** [cryfs/cryfs-web-next/CLAUDE.md](https://github.com/cryfs/cryfs-web-next/blob/fd4b5ce3625a418ea30f3ea0b3e936557476f4ba/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CryFS Website Repository

This is the source code for the CryFS website (https://www.cryfs.org).

## Repository Structure

This is a monorepo with two independent projects:

- **`frontend/`** - Next.js static website (deployed to GitHub Pages)
- **`backend/`** - AWS Lambda serverless functions (deployed to AWS)

Each directory has its own `package.json`, dependencies, and `CLAUDE.md` with detailed guidance.

## Branch

- `master` is the main branch

## Quick Reference

### Frontend
```bash
cd frontend
npm install
npm run dev      # Development server at localhost:3000
npm test         # Unit tests
npm run test:e2e # E2E tests
npm run build    # Production build
```

### Backend
```bash
cd backend
npm install
npm run typecheck # Type checking
npm test          # Unit tests
npm run build     # Build with SAM
npm run local     # Local API server (requires Docker)
npm run deploy    # Deploy to AWS (requires credentials)
```

## Deployment

- **Frontend**: Automatically deployed to GitHub Pages on push to `master`
- **Backend**: Automatically deployed to AWS Lambda on push to `master` (requires AWS secrets in GitHub)

## See Also

- [frontend/CLAUDE.md](frontend/CLAUDE.md) - Frontend
```

</details>
