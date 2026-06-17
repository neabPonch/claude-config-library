---
name: longyangxi__OpenOffice
source: https://github.com/longyangxi/OpenOffice/blob/677285a6a74ea8e621fde27dcc20659256b9a5a7/CLAUDE.md
repo: longyangxi/OpenOffice
kind: claude-md
stars: 221
last_pushed: 2026-04-10T19:39:31Z
license: unknown
score: 8
domains: [agents-ai, cli-tools, devops]
tags: [monorepo, worktree-isolation, state-machine]
curated: 2026-06-15
curated_by: config-scout
---

# longyangxi/OpenOffice — claude-md

**Why it's worth keeping:** The 'Worktree Isolation' and 'Team Execution Flow' sections provide high-density operational logic that prevents an agent from polluting the main repository during development.

**Summary:** Defines a sophisticated multi-agent workspace with strict protocols for file systems, state machines, and git worktree isolation.

**Source credibility:** Decent social proof with 221 stars and recent maintenance activity.

**Recency:** Very current, referencing Next.js 15 and modern tech stacks.

**Source:** [longyangxi/OpenOffice/CLAUDE.md](https://github.com/longyangxi/OpenOffice/blob/677285a6a74ea8e621fde27dcc20659256b9a5a7/CLAUDE.md) · 221★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Open Office

## Project Structure
- `apps/web` - Next.js 15 PWA (Vercel deployment)
- `apps/gateway` - Mac daemon (Node.js + multi-channel + AI CLI control)
- `packages/shared` - Shared event protocol (Zod schemas)
- `packages/orchestrator` - Multi-agent engine (worktree, delegation, phases)
- `packages/memory` - Persistent agent memory (sessions, facts, shared knowledge)

## Git
- All git commit messages MUST be in English.

## Key Commands
- `pnpm dev:web` - Start web dev server
- `pnpm dev:gateway` - Start gateway

## Architecture
- **Channels**: WebSocket (always), Ably (optional), Telegram (optional)
- **UI**: PixiJS v8 pixel office + Key Node Mode agent cards

## Data Directory
- Dev: `~/.open-office-dev/`, Release: `~/.open-office/`
- `config.json` — global config
- `data/instances/<id>/` — per-gateway state (logs, sessions, memory)
- `data/agents.json` — agent definitions
- `projects/` — default agent workspace (team projects created here)
- `worktrees/<repo-hash>/<agentId>/` — centralized worktree isolation

## Worktree Isolation
- One agent = one worktree = one branch (keyed by agentId, not taskId)
- Worktrees stored outside repo at `~/.open-office[-dev]/worktrees/` to
```

</details>
