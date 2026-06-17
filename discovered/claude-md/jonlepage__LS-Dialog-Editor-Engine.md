---
name: jonlepage__LS-Dialog-Editor-Engine
source: https://github.com/jonlepage/LS-Dialog-Editor-Engine/blob/9d734cb55a41ff60e1fb9f6fa9f61f029b52dcfa/CLAUDE.md
repo: jonlepage/LS-Dialog-Editor-Engine
kind: claude-md
stars: 0
last_pushed: 2026-04-22T00:41:29Z
license: other
score: 9
domains: [game-engine, systems-programming]
tags: [multi-language, architecture-driven, technical-reference]
curated: 2026-06-14
curated_by: config-scout
---

# jonlepage/LS-Dialog-Editor-Engine — claude-md

**Why it's worth keeping:** It defines 'authoritative' runtimes to resolve cross-language ambiguity and lists explicit design decisions (e.g., no async/timers) to prevent the AI from proposing invalid pattern changes.

**Summary:** Provides highly detailed technical context for a multi-language engine, including strict architectural constraints and language-specific command patterns.

**Source credibility:** The repo has low social proof (0 stars), but the file content shows high professional rigor in technical specification.

**Recency:** Very recent; it is highly optimized for modern agentic workflows requiring specific test-running and dependency knowledge.

**Source:** [jonlepage/LS-Dialog-Editor-Engine/CLAUDE.md](https://github.com/jonlepage/LS-Dialog-Editor-Engine/blob/9d734cb55a41ff60e1fb9f6fa9f61f029b52dcfa/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

LSDE Dialog Engine — multi-runtime callback-driven dialogue graph dispatcher for [LepaSoft Dialogue Editor](https://lepasoft.com). Executes blueprints (scenes, blocks, connections) exported from LSDE. Reference implementation in TypeScript (`lsde-ts/`), with ports in C# (`lsde-csharp/`), C++ (`lsde-cpp/`), and GDScript (`lsde-gdscript/`).

**`PLAN.md` is the single source of truth.** Read it before any implementation or modification.

## Commands (TypeScript — reference implementation)

All commands run from `lsde-ts/`:

```bash
cd lsde-ts
npm test              # Run all 216 Vitest tests
npm run test:watch    # Watch mode
npm run build         # tsc -p tsconfig.build.json → dist/
npm run lint          # Type-check only (tsc --noEmit)
npm run playground    # Interactive test harness (tsx)
```

Run a single test file:

```bash
cd lsde-ts && npx vitest run src/engine.test.ts
```

Run tests matching a pattern:

```bash
cd lsde-ts && npx vitest run -t "pattern"
```

Documentation:

```bash
cd lsde-ts
npm run docs:dev      # VitePress dev server (4 loc
```

</details>
