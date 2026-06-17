---
name: bmarini__jchess
source: https://github.com/bmarini/jchess/blob/01b0c4c97e3a7fc91b05d0258f0d2739e1350b28/CLAUDE.md
repo: bmarini/jchess
kind: claude-md
stars: 83
last_pushed: 2026-04-07T16:32:09Z
license: mit
score: 9
domains: [web-frontend, game-engine]
tags: [architecture-patterns, domain-specific, typescript-strict]
curated: 2026-06-15
curated_by: config-scout
---

# bmarini/jchess — claude-md

**Why it's worth keeping:** It includes a 'Common Gotchas' section for TypeScript strictness and a detailed module map that explains component responsibilities rather than just listing files.

**Summary:** This file provides deep architectural insights, domain-specific logic mappings, and specific technical constraints to prevent AI hallucinations.

**Source credibility:** High-quality documentation in an active, niche open-source repository.

**Recency:** Very recent; updated within the last few months.

**Source:** [bmarini/jchess/CLAUDE.md](https://github.com/bmarini/jchess/blob/01b0c4c97e3a7fc91b05d0258f0d2739e1350b28/CLAUDE.md) · 83★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Context for Claude Code when working in this repository.

## What this project is

jChess is a chess game viewer. It takes PGN-formatted chess games and renders an interactive board. The rewrite (2024) replaced a 2008 jQuery plugin with a modern TypeScript + Vite stack.

## Tech stack

- **TypeScript** — strict mode, `noUncheckedIndexedAccess` enabled
- **Vite** — build tool and dev server
- **Vitest** — tests, co-located as `*.test.ts` beside source files
- No UI framework. No jQuery. No external chess library.

## Commands

```bash
npm run dev          # start dev server (index.html demo)
npm test             # run all tests
npm run test:watch   # watch mode
npm run build        # build to dist/
```

## Source module map

| File | Responsibility |
|---|---|
| `src/types.ts` | All shared types — touch this when adding new data shapes |
| `src/board.ts` | `Position` class (Layer 1: board state), FEN parsing, `applyMove`, `isInCheck`, coordinate helpers, piece vectors, pin detection |
| `src/movegen.ts` | Move generation (Layer 2: SAN translation), `toSAN`, `legalMovesFrom`, `hasAnyLegalMove`. Depends on board.ts only. |
| `src/pgn.ts` | PGN tokenizer + parser. No `eval
```

</details>
