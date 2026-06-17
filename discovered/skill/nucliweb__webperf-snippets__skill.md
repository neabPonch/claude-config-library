---
name: nucliweb__webperf-snippets__skill
source: https://github.com/nucliweb/webperf-snippets/blob/1aa6af4b15a4c180ed5b0271343aa11ce4b50a6e/skills/webperf/SKILL.md
repo: nucliweb/webperf-snippets
kind: skill
stars: 1442
last_pushed: 2026-06-13T10:45:44Z
license: mit
score: 8
domains: [web-frontend, performance-auditing, dev-tools]
tags: [performance, chrome-devtools, mcp]
curated: 2026-06-15
curated_by: config-scout
---

# nucliweb/webperf-snippets — skill

**Why it's worth keeping:** It demonstrates how to map specific natural language triggers to sub-toolsets and provides a precise multi-step MCP workflow (navigate -> evaluate -> interpret) for the agent to follow.

**Summary:** A domain-specific orchestration layer that turns a collection of JS snippets into an actionable web performance auditing agent via Chrome DevTools.

**Source credibility:** Highly credible with 1400+ stars and very recent maintenance.

**Recency:** Current; leverages the modern Model Context Protocol (MCP) pattern essential for modern agents.

**Source:** [nucliweb/webperf-snippets/skills/webperf/SKILL.md](https://github.com/nucliweb/webperf-snippets/blob/1aa6af4b15a4c180ed5b0271343aa11ce4b50a6e/skills/webperf/SKILL.md) · 1442★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: webperf
description: Web performance measurement and debugging toolkit. Use when the user asks about web performance, wants to audit a page, or says "analyze performance", "debug lcp", "check ttfb", "measure core web vitals", "audit images", or similar.
context: fork
license: MIT
metadata:
  author: Joan Leon | @nucliweb
  version: 1.2.0
  mcp-server: chrome-devtools
  category: web-performance
  repository: https://github.com/nucliweb/webperf-snippets
---

# WebPerf Snippets Toolkit

A collection of 49 JavaScript snippets for measuring and debugging web performance in Chrome DevTools. Each snippet runs in the browser console and outputs structured, color-coded results.

## Quick Reference

| Skill | Snippets | Trigger phrases |
|-------|----------|-----------------|
| webperf-core-web-vitals | 7 | "debug LCP", "slow LCP", "CLS", "layout shifts", "INP", "interaction latency", "responsiveness" |
| webperf-loading | 29 | "TTFB", "slow server", "FCP", "render blocking", "font loading", "script loading", "resource hints", "service worker" |
| webperf-interaction | 9 | "jank", "scroll performance", "long tasks", "animation frames", "INP debug" |
| webperf-media | 3 | "image au
```

</details>
