---
name: michael__editable-website
source: https://github.com/michael/editable-website/blob/1c9a84c2c90cb0e95596e830d4063dd70b0297e6/CLAUDE.md
repo: michael/editable-website
kind: claude-md
stars: 1727
last_pushed: 2026-06-14T22:53:23Z
license: unknown
score: 9
domains: [web-frontend, svelte]
tags: [strict-constraints, mcp-orchestration, workflow-management]
curated: 2026-06-15
curated_by: config-scout
---

# michael/editable-website — claude-md

**Why it's worth keeping:** Uses 'negative constraints' to prevent agent overreach/refactoring drift and provides explicit, multi-step tool orchestration instructions.

**Summary:** Provides rigorous operational constraints to prevent feature creep and maintain architectural integrity during development. It also includes detailed workflows for interacting with specialized MCP tools.

**Source credibility:** High; derived from a popular repository with recent activity and clear domain expertise.

**Recency:** Very current; utilizes modern Svelte 5 patterns and advanced MCP-driven workflows.

**Source:** [michael/editable-website/CLAUDE.md](https://github.com/michael/editable-website/blob/1c9a84c2c90cb0e95596e830d4063dd70b0297e6/CLAUDE.md) · 1727★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

**Development:**
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

**Implementation Guidelines:**
- Before implementing any feature, read `ARCHITECTURE.md` for design decisions and `IMPLEMENTATION_PLAN.md` for the step-by-step implementation spec
- Design decisions go in `ARCHITECTURE.md`, implementation steps go in `IMPLEMENTATION_PLAN.md`
- New features must be specified before implementation begins — the spec should be concise but sufficient to derive the implementation from
- If a gap in either doc is discovered during implementation, update it with a minimal but concise change before proceeding with the code
- Do exactly what the user asks for — one step at a time
- Do NOT think 4 steps ahead or add extra features/improvements
- Only implement the specific change requested
- You can suggest what the next step could be, but don't implement it
- For anything that runs from the home route (`/`) in no-backend / Vercel mode, do NOT add top-level imports of backend-only modu
```

</details>
