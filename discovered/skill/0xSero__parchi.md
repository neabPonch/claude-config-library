---
name: 0xSero__parchi
source: https://github.com/0xSero/parchi/blob/812e979c0db8ac79e36b9b2e448b858320941ca3/SKILL.MD
repo: 0xSero/parchi
kind: skill
stars: 539
last_pushed: 2026-04-24T23:15:20Z
license: mit
score: 8
domains: [browser-automation, ai-agents, cli-tools]
tags: [browser, rpc, automation]
curated: 2026-06-14
curated_by: config-scout
---

# 0xSero/parchi — skill

**Why it's worth keeping:** Defines a clear RPC surface and specific toolset (getTabs, getContent) that can be directly mapped into an AI's tool-calling capabilities for real-world browser interaction.

**Summary:** Documentation for a local daemon that bridges CLI tool-calling to a browser-based agent via WebSocket/JSON-RPC.

**Source credibility:** High; 500+ stars and recent updates suggest a legitimate, functional developer utility.

**Recency:** Current; updated within the last two months.

**Source:** [0xSero/parchi/SKILL.MD](https://github.com/0xSero/parchi/blob/812e979c0db8ac79e36b9b2e448b858320941ca3/SKILL.MD) · 539★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: parchi-relay
description: Use Parchi Relay to control a real browser via the Parchi extension agent (WebSocket) or directly via JSON-RPC from a CLI/tooling workflow.
---

# Parchi Relay (How To Use It)

This skill documents how to run the Parchi relay daemon, connect the browser extension as an agent, and use the CLI to drive browser automation.

## What You Get

- A local relay daemon (`/v1/rpc` + `/v1/extension`) that brokers calls.
- A browser extension agent that connects to the daemon over WebSocket and executes browser tools.
- A CLI (`parchi-relay` / `npm run relay`) that can:
  - list agents
  - pick the default agent
  - list tools / call tools
  - run an agent task and wait for completion

## Quickstart (Local)

1. Build everything:
```bash
npm install
npm run build
```

2. Start the relay daemon (terminal A):
```bash
npm run relay:daemon -- --token=<YOUR_TOKEN> --host=127.0.0.1 --port=17373
```

3. Load the extension (Chrome):

- Open `chrome://extensions`
- Enable Developer mode
- Load unpacked: `dist/`
- Open the extension sidepanel
- Settings -> Relay:
  - Enable: `On`
  - URL: `http://127.0.0.1:17373`
  - Token: `<YOUR_TOKEN>`
  - Click `Apply`

4. Confirm
```

</details>
