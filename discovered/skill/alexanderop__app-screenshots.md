---
name: alexanderop__app-screenshots
source: https://github.com/alexanderop/app-screenshots/blob/612e31ede8b03154057282578334d1857b7c5bb9/skill.md
repo: alexanderop/app-screenshots
kind: skill
stars: 12
last_pushed: 2026-03-26T19:51:29Z
license: mit
score: 8
domains: [web-frontend, cli-tools, automation]
tags: [screenshots, documentation, browser-automation]
curated: 2026-06-14
curated_by: config-scout
---

# alexanderop/app-screenshots — skill

**Why it's worth keeping:** It utilizes a high-reliability 'validate-before-action' pattern where the agent verifies CSS selectors via injected JS before attempting annotations to prevent broken outputs.

**Summary:** A structured workflow for generating professional, annotated visual documentation of web applications or local development servers.

**Source credibility:** The repository has modest popularity and recent maintenance, suggesting a functional niche utility.

**Recency:** Recent (3 months ago), aligning with modern agentic browser automation standards.

**Source:** [alexanderop/app-screenshots/skill.md](https://github.com/alexanderop/app-screenshots/blob/612e31ede8b03154057282578334d1857b7c5bb9/skill.md) · 12★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: screenshotting-apps
description: >
  Generates annotated screenshot documentation for web apps and websites — local dev servers
  or live sites. Use when asked to "screenshot the app", "document the app", "visual docs",
  "screenshot documentation", "show me the app", "screenshot <url>", or "document this website".
---

# Annotated Screenshot Documentation

Generate a markdown document with annotated screenshots of any web app or live website.

## Prerequisites

- `agent-browser` CLI installed globally (`npm i -g agent-browser && agent-browser install`)

## Phase 1: Determine the Target

### A) Live website

1. Normalize URL (add `https://` if missing):
   ```bash
   agent-browser open https://example.com && agent-browser wait --load networkidle
   ```
2. Dismiss cookie/consent banners using semantic locators (most reliable):
   ```bash
   agent-browser find text "Accept" click
   ```
   Or snapshot to find the accept button ref, then click the ref directly:
   ```bash
   agent-browser snapshot -i -s "[role=dialog], [class*=cookie], [class*=consent]" -c
   agent-browser click @e1  # Use the ref from snapshot
   ```
   Verify it's gone: `agent-browser is visible "[role=dia
```

</details>
