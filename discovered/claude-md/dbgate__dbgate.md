---
name: dbgate__dbgate
source: https://github.com/dbgate/dbgate/blob/6bacb1c81e8e330ca0ee163ec06202b68a1e0591/CLAUDE.md
repo: dbgate/dbgate
kind: claude-md
stars: 7059
last_pushed: 2026-06-16T12:44:48Z
license: gpl-3.0
score: 9
domains: [monorepo, fullstack, database-tools]
tags: [architecture, monorepo, workflow]
curated: 2026-06-17
curated_by: config-scout
---

# dbgate/dbgate — claude-md

**Why it's worth keeping:** The detailed monorepo-to-package mapping and explicit descriptions of internal patterns (like state management and process isolation) are gold standards for AI navigation.

**Summary:** This config provides a comprehensive architectural map of a complex monorepo, detailing package responsibilities and specific development workflows.

**Source credibility:** High; it's a well-starred, actively maintained open-source database tool.

**Recency:** Highly current, referencing modern tools like Rolldown and specific Svelte versions.

**Source:** [dbgate/dbgate/CLAUDE.md](https://github.com/dbgate/dbgate/blob/6bacb1c81e8e330ca0ee163ec06202b68a1e0591/CLAUDE.md) · 7059★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

DbGate is a cross-platform (no)SQL database manager supporting MySQL, PostgreSQL, SQL Server, Oracle, MongoDB, Redis, SQLite, and more. It runs as a web app (Docker/NPM), an Electron desktop app, or in a browser. The monorepo uses Yarn workspaces.

## Development Commands

```sh
yarn          # install all packages (also builds TS libraries and plugins)
yarn start    # run API (port 3000) + web (port 5001) concurrently
```

For more control, run these 3 commands in separate terminals:
```sh
yarn start:api    # Express API on port 3000
yarn start:web    # Svelte frontend on port 5001
yarn lib          # watch-compile TS libraries and plugins
```

For Electron development:
```sh
yarn start:web     # web on port 5001
yarn lib           # watch TS libs/plugins
yarn start:app     # Electron app
```

### Building

```sh
yarn build:lib          # build all TS libraries (sqltree, tools, filterparser, datalib, rest)
yarn build:api          # build API
yarn build:web          # build web frontend
yarn ts                 # TypeScript type-check API and web
```

</details>
