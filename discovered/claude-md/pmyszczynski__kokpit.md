---
name: pmyszczynski__kokpit
source: https://github.com/pmyszczynski/kokpit/blob/13c3a23dcb51d75a57c4a332036241f48d4f73da/Claude.md
repo: pmyszczynski/kokpit
kind: claude-md
stars: 2
last_pushed: 2026-06-11T23:54:54Z
license: mit
score: 9
domains: [web-frontend, fullstack, devops]
tags: [context-gateway, guardrails, hierarchical-docs]
curated: 2026-06-16
curated_by: config-scout
---

# pmyszczynski/kokpit — claude-md

**Why it's worth keeping:** The 'Non-Negotiables' section provides essential guardrails for an agent, and the project structure mapping clearly defines folder responsibilities.

**Summary:** A highly effective 'context gateway' that uses CLAUDE.md as a concise briefing while offloading depth to specialized docs.

**Source credibility:** Low star count (2) but shows high signal-to-noise ratio and professional documentation standards.

**Recency:** Extremely current; uses Next.js 15 and follows modern context-window optimization strategies.

**Source:** [pmyszczynski/kokpit/Claude.md](https://github.com/pmyszczynski/kokpit/blob/13c3a23dcb51d75a57c4a332036241f48d4f73da/Claude.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

> This file is automatically read by Claude Code on every session.
> Keep it as a concise briefing. Full detail lives in `docs/`.

---

## Project Overview

A self-hosted personal dashboard / homepage — a modern alternative to Homepage, Homarr, Dashy, and Heimdall.

**Core goal:** The ultimate configurable homepage for a homelab or personal server. Beautiful by default, infinitely tweakable, secure enough to expose to the internet.

**Key differentiators from existing tools:**
- Dual-config: everything controllable both from a visual in-app UI **and** a `settings.yaml` file (they stay in sync)
- Built-in authentication — no reliance on external reverse proxies for basic protection
- First-class widget/integration system with a clean plugin-like API
- Modern, polished default theme with deep CSS variable support for personalization

---

## Tech Stack

- **Framework:** Next.js 15.x (App Router)
- **Styling:** CSS custom properties (`[data-theme]` attribute) + Tailwind utility layer
- **Config:** YAML (`settings.yaml` at project root / config dir)
- **Auth:** Built-in credential auth (bcrypt), JWT session tokens, optional TOTP 2FA
- **Deployment:** Docker + Docker Compos
```

</details>
