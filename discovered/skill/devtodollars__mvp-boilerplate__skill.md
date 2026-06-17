---
name: devtodollars__mvp-boilerplate__skill
source: https://github.com/devtodollars/mvp-boilerplate/blob/2aac5c2fcb45c35aa4a5f5eb9eb66645f0f84e70/.claude/browser/SKILL.md
repo: devtodollars/mvp-boilerplate
kind: skill
stars: 988
last_pushed: 2026-03-05T19:46:05Z
license: mit
score: 9
domains: [agents-ai, web-automation, cli-tools]
tags: [browser, automation]
curated: 2026-06-15
curated_by: config-scout
---

# devtodollars/mvp-boilerplate — skill

**Why it's worth keeping:** The 'snapshot' system that maps DOM elements to stable IDs (e.g., @e1) is a top-tier technique that prevents agents from failing due to fragile CSS or XPath selectors.

**Summary:** A comprehensive tool-definition for browser automation via the `agent-browser` CLI, covering navigation, interaction, and network interception.

**Source credibility:** High; comes from a highly-starred (988 stars) developer boilerplate repository.

**Recency:** Current; utilizes modern patterns specifically designed for AI agentic web interaction.

**Source:** [devtodollars/mvp-boilerplate/.claude/browser/SKILL.md](https://github.com/devtodollars/mvp-boilerplate/blob/2aac5c2fcb45c35aa4a5f5eb9eb66645f0f84e70/.claude/browser/SKILL.md) · 988★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: browser
description: Automate browser interactions using agent-browser CLI — navigate, click, fill forms, scrape content, take screenshots, and more.
argument-hint: <command> [args...]
allowed-tools: Bash(npx agent-browser *)
---

# Browser Automation with agent-browser

Control a headless Chromium browser via CLI commands. All commands are run with `npx agent-browser <command>`.

## Setup (first time only)

```bash
npx agent-browser install
```

## Navigation

| Command | Description |
|---|---|
| `open <url>` | Navigate to a URL |
| `close` | Close browser |
| `tab` | List open tabs |
| `tab new [url]` | Open new tab |
| `tab <n>` | Switch to tab n |
| `tab close [n]` | Close tab |
| `window new` | Open new browser window |
| `frame <selector>` | Switch to iframe |
| `frame main` | Return to main frame |

## Page Inspection (use these to understand page structure)

| Command | Description |
|---|---|
| `snapshot` | Get accessibility tree with `@e1`, `@e2` element refs (best for AI) |
| `screenshot [path]` | Capture screenshot |
| `screenshot --full` | Full page screenshot |
| `screenshot --annotate` | Screenshot with numbered element labels |
| `get text <sel>` | Extrac
```

</details>
