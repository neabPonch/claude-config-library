---
name: jtrackingai__analytics-tracking-automation
source: https://github.com/jtrackingai/analytics-tracking-automation/blob/68378e000ef24123ddd031d42e95587ef137bd87/SKILL.md
repo: jtrackingai/analytics-tracking-automation
kind: skill
stars: 128
last_pushed: 2026-04-29T10:42:34Z
license: apache-2.0
score: 9
domains: [automation, analytics, cli-tools]
tags: [gtm, ga4, orchestration]
curated: 2026-06-14
curated_by: config-scout
---

# jtrackingai/analytics-tracking-automation — skill

**Why it's worth keeping:** Uses advanced agentic patterns including self-updating logic, artifact-driven state routing, and a strict 'Shared Contract' for privacy/telemetry handling.

**Summary:** An orchestrator skill that manages end-to-end GA4 and GTM implementation through specialized sub-phases like discovery, schema generation, and sync.

**Source credibility:** High; well-maintained repository with significant community interest (128 stars).

**Recency:** Very current; includes modern requirements for Playwright automation and OAuth loopback callbacks.

**Source:** [jtrackingai/analytics-tracking-automation/SKILL.md](https://github.com/jtrackingai/analytics-tracking-automation/blob/68378e000ef24123ddd031d42e95587ef137bd87/SKILL.md) · 128★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: analytics-tracking-automation
description: Use when you need GA4 + GTM tracking delivery from site discovery through publish, or when the right phase entry point is still unclear.
compatibility: >
  Requires Node.js 18+, npm, and Playwright Chromium for browser-backed steps.
  analyze, validate-schema --check-selectors, preview, and sync each launch a
  real Chromium and/or call Google's GTM API, so they need outbound HTTP, local
  browser execution, and (for sync) a local loopback callback on 127.0.0.1 to
  receive Google's OAuth consent redirect. Run them in an environment that
  provides those capabilities. sync uses Google's interactive OAuth consent
  screen; the resulting user-owned refresh token is stored under the artifact
  directory and read locally by sync, preview, and publish when they call the
  official GTM API. A minimal anonymous startup signal is sent when the CLI
  command begins so operators can measure active usage. Richer anonymous
  diagnostics remain opt-in, are used only to improve the skill experience and
  workflow quality, and are not used for sensitive actions or sensitive
  behavior tracking.
---

# Analytics Tracking Automation

Use this ski
```

</details>
