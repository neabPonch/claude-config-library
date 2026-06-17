---
name: tuanngocptn__nport
source: https://github.com/tuanngocptn/nport/blob/3b62b831764662df3e2df2244df7a749c3847789/CLAUDE.md
repo: tuanngocptn/nport
kind: claude-md
stars: 502
last_pushed: 2026-04-01T04:27:57Z
license: mit
score: 9
domains: [cli-tools, typescript, backend]
tags: [procedural-recipes, architecture-map, esm-rules]
curated: 2026-06-15
curated_by: config-scout
---

# tuanngocptn/nport — claude-md

**Why it's worth keeping:** Uses 'How to add...' procedural recipes that teach the agent how to extend the app; highlights critical technical nuances like ESM '.js' import requirements.

**Summary:** Provides a clear breakdown of a multi-component system (CLI/Server/Binary) including traffic flow and command sets.

**Source credibility:** High: 502 stars and recent maintenance activity.

**Recency:** Current: follows modern TypeScript/ESM standards.

**Source:** [tuanngocptn/nport/CLAUDE.md](https://github.com/tuanngocptn/nport/blob/3b62b831764662df3e2df2244df7a749c3847789/CLAUDE.md) · 502★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

See also `.claude/rules/` for detailed per-topic rules (TypeScript style, patterns, common tasks, project overview).

## Project Overview

NPort is a free, open-source ngrok alternative that creates secure HTTP/HTTPS tunnels from localhost to public URLs using Cloudflare's global edge network. It has three components:

1. **CLI** (`src/`) — TypeScript command-line tool bundled via esbuild
2. **Backend** (`server/`) — Cloudflare Worker that manages tunnel lifecycle (creates/deletes tunnels + DNS via Cloudflare APIs)
3. **cloudflared binary** (`bin/`) — Downloaded at install/first-run; handles the actual tunnel connection

Traffic flow: Browser → `myapp.nport.link` → Cloudflare Edge → cloudflared → `localhost:port`

---

## Commands

### CLI (root directory)

```bash
npm install        # Installs deps + downloads cloudflared (postinstall hook)
npm run build      # esbuild → dist/index.js
npm run dev        # esbuild --watch (fast, no minification)
npm start          # node dist/index.js
npm test           # vitest run (tests/**/*.test.ts)
npm run test:watch # vitest --
```

</details>
