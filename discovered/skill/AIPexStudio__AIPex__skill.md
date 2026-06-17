---
name: AIPexStudio__AIPex__skill
source: https://github.com/AIPexStudio/AIPex/blob/0ad38bf820af48ec06eba06cfc97eab347880bfa/skill/SKILL.md
repo: AIPexStudio/AIPex
kind: skill
stars: 1212
last_pushed: 2026-05-18T11:22:47Z
license: mit
score: 9
domains: [agents-ai, browser-automation, mcp-bridge]
tags: [browser-control, mcp, automation, chrome]
curated: 2026-06-15
curated_by: config-scout
---

# AIPexStudio/AIPex — skill

**Why it's worth keeping:** The 'Tool Usage Strategy' is exceptional; it instructs the agent on a priority-based decision tree (UID-based interaction vs. costly screenshot fallback) to optimize token costs and latency.

**Summary:** Provides a sophisticated MCP bridge connection between AI agents and a Chrome extension for advanced browser automation. It includes setup instructions for multiple IDEs/CLI tools and specific workflows.

**Source credibility:** Highly credible with 1200+ stars and recent maintenance activity.

**Recency:** Current, explicitly mentioning Claude Code CLI and modern MCP clients like Windsurf.

**Source:** [AIPexStudio/AIPex/skill/SKILL.md](https://github.com/AIPexStudio/AIPex/blob/0ad38bf820af48ec06eba06cfc97eab347880bfa/skill/SKILL.md) · 1212★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: aipex-browser
description: AI-powered browser automation using the AIPex Chrome Extension via MCP bridge. Use this skill when the agent needs to control a Chrome browser — navigating pages, clicking elements, filling forms, capturing screenshots, managing tabs, or downloading content — by connecting to the AIPex MCP bridge.
version: 1.0.0
metadata:
  openclaw:
    requires:
      bins:
        - npx
    emoji: "🌐"
    homepage: https://aipex.ai
    os: [macos, linux, windows]
---

# AIPex Browser Control

AIPex is a Chrome extension that exposes 30+ browser automation tools over the Model Context Protocol (MCP). Once connected, the agent can control any Chrome tab using natural language — clicking, typing, navigating, capturing screenshots, downloading content, and more.

**Architecture:**
```
Agent (MCP client) ──stdio──▶ aipex-mcp-bridge ──WebSocket──▶ AIPex Chrome Extension ──▶ Browser APIs
```

---

## When to Use This Skill

Use this skill when the user wants to:

- Navigate to URLs, click links, fill forms, or interact with any web page
- Automate multi-step browser workflows
- Extract or download data from web pages
- Capture screenshots of browser tabs
- Manage mu
```

</details>
