---
name: browser-use__browser-harness-js
source: https://github.com/browser-use/browser-harness-js/blob/95b7a22a923714c45d2f7234b2bfa8fa6322c2eb/SKILL.md
repo: browser-use/browser-harness-js
kind: skill
stars: 463
last_pushed: 2026-04-20T18:47:32Z
license: mit
score: 9
domains: [agents-ai, cli-tools, web-automation]
tags: [cdp, chrome, browser-automation, stateful]
curated: 2026-06-14
curated_by: config-scout
---

# browser-use/browser-harness-js — skill

**Why it's worth keeping:** The auto-detection of running browser profiles is highly sophisticated; the architecture of a long-lived background process to circumvent stateless tool calls is a brilliant pattern for browser automation.

**Summary:** Provides a persistent, stateful bridge to any Chromium-based browser via the DevTools Protocol (CDP) using a background Bun server. It enables an agent to maintain session state and globals across multiple discrete CLI tool calls.

**Source credibility:** Strong; part of a trending 'browser-use' ecosystem with significant GitHub interest and recent maintenance.

**Recency:** Very current, utilizing modern Bun-based execution and up-to-date CDP protocols.

**Source:** [browser-use/browser-harness-js/SKILL.md](https://github.com/browser-use/browser-harness-js/blob/95b7a22a923714c45d2f7234b2bfa8fa6322c2eb/SKILL.md) · 463★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cdp
description: Drive Chrome via the DevTools Protocol from JavaScript. Run JS snippets through the `browser-harness-js` CLI — it auto-spawns a long-lived bun HTTP server holding a fully-typed CDP `Session`, and every call (`browser-harness-js 'await session.Page.navigate(...)'`) executes against the same persistent connection. Session, active target, and globals survive across calls. Use when the user wants to automate, script, or inspect a Chrome browser via CDP — single tab or multi-tab, attach to existing Chrome or to a new one launched with --remote-debugging-port.
---

# CDP — `browser-harness-js` skill

Custom codegen'd CDP SDK (every method from browser_protocol.json + js_protocol.json gets a typed wrapper) plus a tiny HTTP server that holds one persistent CDP `Session`. The `browser-harness-js` CLI auto-starts the server on first use and forwards JS snippets to it.

The SDK lives in the skill's `sdk/` directory. In the rest of this doc, `<skill-dir>` refers to wherever `npx skills add` installed the skill (Claude Code: `~/.claude/skills/cdp`; Cursor: `~/.cursor/skills/cdp`; other agents vary). The CLI should be on PATH as `browser-harness-js`.

## Setup (once, f
```

</details>
