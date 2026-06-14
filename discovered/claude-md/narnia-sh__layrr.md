---
name: narnia-sh__layrr
source: https://github.com/narnia-sh/layrr/blob/e4e7a0ab972d3df4f5acc6a5929f36f3def89c59/CLAUDE.md
repo: narnia-sh/layrr
kind: claude-md
stars: 258
last_pushed: 2026-05-10T06:35:30Z
license: mit
score: 8
domains: [cli-tools, agents-ai, web-proxy]
tags: [architecture-mapping, scope-control, typescript]
curated: 2026-06-14
curated_by: config-scout
---

# narnia-sh/layrr — claude-md

**Why it's worth keeping:** The 'CLI Architecture' section is excellent for mapping specific responsibilities to file paths, and it uses negative constraints to prevent Claude from trying to restore deleted legacy code.

**Summary:** Defines a CLI-only project scope and provides a functional map of the system architecture.

**Source credibility:** Decent mid-sized project with active maintenance (last push 1 month ago).

**Recency:** Current; utilizes modern tooling like pnpm and TypeScript.

**Source:** [narnia-sh/layrr/CLAUDE.md](https://github.com/narnia-sh/layrr/blob/e4e7a0ab972d3df4f5acc6a5929f36f3def89c59/CLAUDE.md) · 258★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code when working with this repository.

## Scope

Layrr is kept as a CLI-only project. The hosted dashboard, process manager, deployment files, templates, and hosted-only agents are intentionally removed.

The repository root is the CLI package.

## Commands

```bash
pnpm install
pnpm build
```

Local CLI run after building:

```bash
node dist/cli.js --port 3000
```

There are no automated tests configured.

## CLI Architecture

The CLI proxies a local dev server, injects a browser overlay, resolves selected elements back to source code, sends edit requests to an AI agent, and records successful edits in git.

Important paths:

- `src/cli.ts` - argument parsing, agent selection, git preflight, proxy startup, edit loop
- `src/agents/` - public agent integrations for Claude Code, Codex, and Gemini via Pi
- `src/server/` - HTTP proxy, WebSocket handling, edit queue, version history
- `src/editor/source-mapper.ts` - source file and line resolution
- `overlay/` - injected browser UI, bundled as an IIFE
- `scripts/build.ts` - builds overlay, compiles TypeScript, copies font assets

## Notes

- Public agents are `claude`, `codex`, and `g
```

</details>
