---
name: Pabreetzio__metasquares
source: https://github.com/Pabreetzio/metasquares/blob/6166e04f9a8ce1bf3d523015ae0f45c0ba03eba9/CLAUDE.MD
repo: Pabreetzio/metasquares
kind: claude-md
stars: 1
last_pushed: 2026-01-16T21:11:45Z
license: mit
score: 8
domains: [web-frontend, mobile-app, monorepo]
tags: [monorepo, game-logic, tanstack, expo]
curated: 2026-06-16
curated_by: config-scout
---

# Pabreetzio/metasquares — claude-md

**Why it's worth keeping:** The directory tree provides immediate spatial awareness for multi-package navigation; the deep dive into the 'useGameLogic' hook prevents the AI from getting lost in implementation details when working on high-level features.

**Summary:** Provides a detailed structural map of a complex monorepo alongside explicit high-level explanations of the core game logic. It bridges the gap between file location awareness and algorithmic understanding.

**Source credibility:** Single developer learning project with low star count.

**Recency:** Very recent, utilizing modern stacks like TanStack Start and React 19.

**Source:** [Pabreetzio/metasquares/CLAUDE.MD](https://github.com/Pabreetzio/metasquares/blob/6166e04f9a8ce1bf3d523015ae0f45c0ba03eba9/CLAUDE.MD) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Metasquares - Project Guide for Claude

## Project Overview

Metasquares is a **monorepo** containing both web and mobile implementations of the abstract strategy game MetaSquares (originally created by Scott Kim in 1996). This is a turn-based two-player game where players compete to form squares on an 8x8 grid, earning points based on the size of squares formed.

**Live Site (Web)**: https://metasquares.graham.tech

## Monorepo Structure

This is an **npm workspaces monorepo** with the following structure:

```
C:\Projects\metasquares\
├── apps/
│   ├── web/                 # TanStack Start web application
│   │   ├── src/
│   │   │   ├── components/  # React components
│   │   │   │   ├── Game.tsx         # Main game logic and state management
│   │   │   │   ├── GameBoard.tsx    # Visual board rendering
│   │   │   │   ├── BoardWell.tsx    # Individual well/cell on the board
│   │   │   │   ├── PlayerMarble.tsx # Visual representation of player markers
│   │   │   │   └── WellHitbox.tsx   # Click detection for wells
│   │   │   ├── routes/      # TanStack Router routes
│   │   │   │   ├── index.tsx        # Home page with game
│   │   │   │   └── _authed/         # Protected r
```

</details>
