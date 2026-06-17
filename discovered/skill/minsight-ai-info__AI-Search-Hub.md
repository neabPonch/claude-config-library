---
name: minsight-ai-info__AI-Search-Hub
source: https://github.com/minsight-ai-info/AI-Search-Hub/blob/afcc7411335c8b194e309f06af7d189448d0b0e2/SKILL.md
repo: minsight-ai-info/AI-Search-Hub
kind: skill
stars: 1171
last_pushed: 2026-04-27T07:47:18Z
license: unknown
score: 8
domains: [agents-ai, web-automation, cli-tools]
tags: [playwright, browser-control, routing-logic, session-management]
curated: 2026-06-15
curated_by: config-scout
---

# minsight-ai-info/AI-Search-Hub — skill

**Why it's worth keeping:** Includes a high-value 'Routing Strategy' table for intent-based tool selection and offers a robust technical pattern for bypassing login/session hurdles in web automation.

**Summary:** Provides instructions for an agent to orchestrate browser-based searches across multiple AI platforms by bridging local authenticated sessions via Chrome DevTools ports.

**Source credibility:** High; 1.1k+ stars and recently updated (2 months ago) indicates a popular, active utility.

**Recency:** Current; utilizes modern Playwright and CDP patterns compatible with modern agentic workflows.

**Source:** [minsight-ai-info/AI-Search-Hub/SKILL.md](https://github.com/minsight-ai-info/AI-Search-Hub/blob/afcc7411335c8b194e309f06af7d189448d0b0e2/SKILL.md) · 1171★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ai-search-hub
description: Run the AI Search Hub browser automation scripts for Yuanbao, LongCat, Doubao, Qwen, Gemini, Grok, and MiniMax. Use this skill when the user wants to ask one of those sites a prompt, auto-start or attach to a Chrome DevTools session on port 9222, seed an isolated debug browser profile from the user's local browser data, detect whether login is required, wait for the user to finish logging in if needed, and then continue automatically.
---

# AI Search Hub

Use this skill only for this repository's AI Search Hub browser automation scripts:

- `scripts/yuanbao_playwright.py`
- `scripts/longcat_playwright.py`
- `scripts/doubao_playwright.py`
- `scripts/qwen_playwright.py`
- `scripts/gemini_playwright.py`
- `scripts/grok_playwright.py`
- `scripts/minimaxi_playwright.py`

## When To Use

Use this skill when the user asks to:

- run one of the supported chat sites from this repo
- normalize invocation across the three scripts
- auto-start a debug Chromium-family browser session
- detect whether `127.0.0.1:9222` is available
- prompt for login if the target site is not logged in, then continue automatically
- seed an isolated debug profile from the use
```

</details>
