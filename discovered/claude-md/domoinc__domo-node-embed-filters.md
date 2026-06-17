---
name: domoinc__domo-node-embed-filters
source: https://github.com/domoinc/domo-node-embed-filters/blob/7fba181a806066f82288f43dd7ad4bf8bbb8402b/CLAUDE.md
repo: domoinc/domo-node-embed-filters
kind: claude-md
stars: 18
last_pushed: 2026-06-03T21:08:33Z
license: mit
score: 9
domains: [backend-api, web-integration]
tags: [node.js, express, auth]
curated: 2026-06-14
curated_by: config-scout
---

# domoinc/domo-node-embed-filters — claude-md

**Why it's worth keeping:** It includes specific JSON payload schemas and detailed RPC method mappings required for maintaining complex integration logic.

**Summary:** Provides a comprehensive architectural map of the Domo embedding lifecycle and MessageChannel communication protocols.

**Source credibility:** High; provided by an official example repository with recent updates.

**Recency:** Current; tailored specifically for Claude Code context usage.

**Source:** [domoinc/domo-node-embed-filters/CLAUDE.md](https://github.com/domoinc/domo-node-embed-filters/blob/7fba181a806066f82288f43dd7ad4bf8bbb8402b/CLAUDE.md) · 18★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Node.js Express demonstration application showing how to implement Domo private embedding with programmatic filtering. The app uses OAuth2 for Domo API authentication, generates secure embed tokens, and demonstrates two-way communication between parent pages and embedded Domo content via MessageChannel postMessage API.

## Development Commands

```bash
# Install dependencies (use Yarn, as project has yarn.lock)
yarn install

# Start development server (default port 3001)
yarn start

# Start on custom port
yarn start -p 4000

# Alternative using npm (though Yarn is preferred)
npm start
```

**Note**: This repository has no test suite, linting, or build process configured.

## Configuration

Required `.env` file (copy from `.env.example`):
- `CLIENT_ID` / `CLIENT_SECRET`: Domo OAuth credentials from developer account
- `EMBED_ID`: Dashboard/card/page ID to embed
- `EMBED_TYPE`: One of `dashboard`, `card`, or `page`

Optional settings:
- `USE_XHR=true`: Switches from standard iframe to XHR-based embedding (serves `sample_xhr.html` instead
```

</details>
