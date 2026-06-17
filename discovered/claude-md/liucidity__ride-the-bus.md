---
name: liucidity__ride-the-bus
source: https://github.com/liucidity/ride-the-bus/blob/27be29065f38d922c28da3e5ba54b6dab61174d4/CLAUDE.md
repo: liucidity/ride-the-bus
kind: claude-md
stars: 1
last_pushed: 2026-04-22T00:01:33Z
license: unknown
score: 8
domains: [web-frontend, real-time-communications, game-development]
tags: [monorepo, socket.io, architecture-mapping]
curated: 2026-06-14
curated_by: config-scout
---

# liucidity/ride-the-bus — claude-md

**Why it's worth keeping:** The Socket.io event table and explicit game state/reducer action listings are perfect patterns for documenting asynchronous communication flows to an AI.

**Summary:** Provides a high-density architectural map for a real-time, multi-app monorepo.

**Source credibility:** Low star count (1), likely a personal project or portfolio piece.

**Recency:** Current; useful for modern agent-driven development workflows.

**Source:** [liucidity/ride-the-bus/CLAUDE.md](https://github.com/liucidity/ride-the-bus/blob/27be29065f38d922c28da3e5ba54b6dab61174d4/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Is

**Ride The Bus** is a party card game web app with a 3-app monorepo:

- **client** (port 3000) — Host/display interface for the game (React + TypeScript)
- **player-client** (port 4000) — Mobile controller for players (React + TypeScript)
- **server** (port 3001) — WebSocket game server (Express + Socket.io)

Cards are sourced from the external [Deck of Cards API](https://www.deckofcardsapi.com/). No database; all game state is in-memory per session.

## Commands

Each app is run independently:

```bash
# Server
cd server && node express.js

# Client (host display)
cd client && npm start        # dev server
cd client && npm run build    # production build
cd client && npm test         # run tests

# Player client (mobile controller)
cd player-client && npm start
cd player-client && npm run build
cd player-client && npm test
```

## Architecture

### Game Flow

1. Players join via `player-client` by entering a username (sent as `enterRoom` socket event)
2. Host (client) draws 4 cards per round via the Deck of Cards API
3. Each round, players guess on
```

</details>
