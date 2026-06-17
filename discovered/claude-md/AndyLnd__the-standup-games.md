---
name: AndyLnd__the-standup-games
source: https://github.com/AndyLnd/the-standup-games/blob/5c45ab017938364a38b9d5508c77587e7e1b01e1/claude.md
repo: AndyLnd/the-standup-games
kind: claude-md
stars: 6
last_pushed: 2026-02-14T16:48:32Z
license: unknown
score: 9
domains: [web-frontend, multiplayer-games, real-time]
tags: [svelte-5, colyseus, monorepo, websocket]
curated: 2026-06-16
curated_by: config-scout
---

# AndyLnd/the-standup-games — claude-md

**Why it's worth keeping:** Includes specific 'Adding a New Game' workflows and explicit Svelte 5 Runes syntax mappings to prevent LLM hallucination of deprecated patterns.

**Summary:** Provides high-density technical context for a complex real-time multiplayer monorepo using Svelte 5 and Colyseus.

**Source credibility:** High-quality, dense documentation suggests a sophisticated developer despite low star count.

**Recency:** 

**Source:** [AndyLnd/the-standup-games/claude.md](https://github.com/AndyLnd/the-standup-games/blob/5c45ab017938364a38b9d5508c77587e7e1b01e1/claude.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# standup.games

Multiplayer real-time game platform for team standups and remote team building.

**Website**: https://www.thestandup.games

## Tech Stack

- **Frontend**: SvelteKit 2 + Svelte 5 (Runes) + TypeScript + Vite 7
- **Backend**: Express 5 + Colyseus 0.16 (WebSocket multiplayer framework)
- **State Sync**: @colyseus/schema 3.x (binary serialization)
- **Monorepo**: npm workspaces + Turborepo
- **Deployment**: Docker (Node 22-alpine)

## Project Structure

```
standup.games/
├── apps/
│   ├── client/          # SvelteKit frontend (port 5173)
│   │   └── src/routes/  # File-based routing
│   └── server/          # Express + Colyseus backend (port 2567)
│       └── src/
│           ├── index.ts
│           └── arena.config.ts  # Room definitions
├── games/
│   ├── rumble/          # Battle royale game (production-ready)
│   │   ├── server/      # Game room + schema
│   │   ├── client/      # Svelte components + store
│   │   └── types/       # Generated types from schema
│   ├── slimevolley/     # Volleyball game (in development)
│   │   ├── server/
│   │   └── client/
│   └── utils/           # Shared utilities (vec.ts, keyhandler.ts)
└── packages/
    ├── eslint-config-cus
```

</details>
