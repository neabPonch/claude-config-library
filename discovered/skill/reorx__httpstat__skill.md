---
name: reorx__httpstat__skill
source: https://github.com/reorx/httpstat/blob/b37cd4655c0b0595dbf5be4466abd1dcbc202b84/skills/httpstat/SKILL.md
repo: reorx/httpstat
kind: skill
stars: 6211
last_pushed: 2026-04-08T10:04:34Z
license: mit
score: 9
domains: [cli-tools, network, backend-api, devops]
tags: [http, performance, latency, diagnostics]
curated: 2026-06-15
curated_by: config-scout
---

# reorx/httpstat — skill

**Why it's worth keeping:** It encodes domain expertise by providing specific timing thresholds and 'next-step' instructions based on the bottleneck detected. The intent-based triggering logic is also excellent, capturing user requests about 'slowness' even without tool names.

**Summary:** Provides a comprehensive diagnostic framework for HTTP latency analysis using httpstat. It converts raw timing data into actionable expert troubleshooting steps.

**Source credibility:** High; based on a well-regarded, actively maintained open-source utility.

**Recency:** Current; includes modern installation workflows like `uv` and standard CLI patterns.

**Source:** [reorx/httpstat/skills/httpstat/SKILL.md](https://github.com/reorx/httpstat/blob/b37cd4655c0b0595dbf5be4466abd1dcbc202b84/skills/httpstat/SKILL.md) · 6211★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: httpstat
description: >
  Diagnose website and API performance using httpstat — a curl wrapper that visualizes
  HTTP timing breakdowns (DNS, TCP, TLS, server processing, content transfer).
  Use this skill whenever the user wants to debug slow websites, analyze HTTP/HTTPS
  latency, profile API response times, understand curl timing output, find network
  bottlenecks, check TLS handshake speed, measure Time to First Byte (TTFB), or
  troubleshoot any connection performance issue. Also trigger when the user has a
  curl command and wants to understand where time is being spent, or when they paste
  httpstat output and want help interpreting it. Even if the user doesn't mention
  "httpstat" by name — if they're asking "why is this endpoint slow?" or "what's
  taking so long?" for an HTTP request, this skill applies.
---

# httpstat: HTTP Performance Diagnostics

Use `httpstat` — a curl wrapper that breaks down HTTP request timing into discrete
phases — to diagnose where latency lives and what to do about it.

## When to use httpstat

- User says a website or API is slow
- User wants to profile an HTTP endpoint
- User has a curl command and wants timing visibility
- User as
```

</details>
