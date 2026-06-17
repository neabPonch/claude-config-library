---
name: mikenjuki__daibug
source: https://github.com/mikenjuki/daibug/blob/cfd7d05bff2a402af1e736d37a8d0d78828b2e13/Claude.md
repo: mikenjuki/daibug
kind: claude-md
stars: 0
last_pushed: 2026-02-24T16:29:44Z
license: unknown
score: 9
domains: [cli-tools, web-extensions, debugging]
tags: [post-mortem, regression-prevention, technical-debt]
curated: 2026-06-14
curated_by: config-scout
---

# mikenjuki/daibug — claude-md

**Why it's worth keeping:** Uses the 'What Fixed [ISS-XXX]' pattern to encode tribal knowledge and specific architectural failure modes directly into the agent's context.

**Summary:** Combines project architecture with a 'living post-mortem' of recent bug fixes to prevent regression.

**Source credibility:** Low star count, but content shows high technical depth in systems/extension development.

**Recency:** Highly current; utilizes the latest patterns for agentic development and system state tracking.

**Source:** [mikenjuki/daibug/Claude.md](https://github.com/mikenjuki/daibug/blob/cfd7d05bff2a402af1e736d37a8d0d78828b2e13/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Daibug - Agent Guidelines

## Project Overview

Daibug is a browser-to-CLI AI debugging bridge. It has:
- Hub: `src/hub.ts` (HTTP + WebSocket)
- Extension: `extension/` (console/network/DOM capture)
- Agent Bridge: `src/agent-bridge.ts`

## Known Issues First

Before touching extension or Playwright code, read `docs/issues.md`.

Current state (2026-02-19):
- No open Phase 2 issues.
- `npm run test:e2e` -> 21/21 passing
- `npm test` -> 213/213 passing

## What Fixed ISS-005 (for next time)

Problem was 5 failures in `tests/phase2/e2e-dom-react-reconnect.test.ts`.

Fixes applied:

1. Command flow Hub -> extension -> page
- File: `extension/background.js`
- WS commands now relay to localhost tabs via `chrome.tabs.sendMessage(...)`
- This replaced background `chrome.runtime.sendMessage(...)` for command fanout

2. Faster reconnect/discovery
- File: `extension/background.js`
- `DISCOVERY_INTERVAL` reduced to `500ms`
- Added discovery trigger on localhost tab updates

3. React tree capture robustness
- File: `extension/page-context.js`
- Added safe `window.__REACT_DEVTOOLS_GLOBAL_HOOK__` shim
- `capture_react` now tries fiber roots first, then marker fallback

4. Removed CDN dependency
```

</details>
