---
name: memrynote__memry
source: https://github.com/memrynote/memry/blob/0dfc576eab58240c7fec664d5c9ae5fd3ccdbacf/CLAUDE.md
repo: memrynote/memry
kind: claude-md
stars: 30
last_pushed: 2026-06-14T19:22:02Z
license: gpl-3.0
score: 9
domains: [desktop-app, monorepo, security, local-first]
tags: [electron, monorepo, verification-workflows, architecture-constraints]
curated: 2026-06-15
curated_by: config-scout
---

# memrynote/memry — claude-md

**Why it's worth keeping:** Uses high-leverage sections like 'Known Gotchas' for native module issues, explicit efficiency budgets (tool call limits), and mandatory verification workflows (IPC/docs impact) that prevent common LLM regression patterns.

**Summary:** A dense technical manual that integrates build/test commands with architectural constraints (CRDT/E2E) and strict verification protocols. It provides the agent with deep context on both how to execute tasks and how to prevent breaking changes in a complex monorepo.

**Source credibility:** High; written by a developer of a specialized local-first tool with specific technical depth.

**Recency:** Very current; uses modern dependencies like Electron 39 and VitePress.

**Source:** [memrynote/memry/CLAUDE.md](https://github.com/memrynote/memry/blob/0dfc576eab58240c7fec664d5c9ae5fd3ccdbacf/CLAUDE.md) · 30★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file backs `AGENTS.md`; `AGENTS.md` is a symlink to `CLAUDE.md`.

Kaan owns this. Start: say hi + one motivating line. Work style: telegraph; noun phrases ok; drop grammar; min tokens.

Research the codebase before editing. Never change code you haven't read.

## Build & Dev

```bash
pnpm dev          # Electron desktop app
pnpm dev:desktop  # desktop through turbo
pnpm dev:landing  # landing site
pnpm dev:sync-server # sync server
pnpm docs:dev     # docs site
pnpm --filter @memry/desktop dev:a # desktop profile/device A
pnpm --filter @memry/desktop dev:b # desktop profile/device B
pnpm --filter @memry/desktop dev:c # desktop profile/device C
```

## Verify

```bash
pnpm lint         # ESLint (flat config)
pnpm typecheck    # TypeScript across all packages
pnpm test         # Vitest (desktop + sync-server via turbo)
pnpm test:desktop # desktop tests only
pnpm test:sync-server # sync-server tests only
pnpm test:e2e     # Playwright E2E (Electron)
pnpm check:architecture # architecture boundary check
pnpm check:contracts # contract boundary check
pnpm docs:impact --base origin/main --strict # docs gate for desktop/sync changes
pnpm docs:build   # VitePress docs bui
```

</details>
