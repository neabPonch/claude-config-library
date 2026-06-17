---
name: HatcherLabs__hatcher-skill
source: https://github.com/HatcherLabs/hatcher-skill/blob/d7a6a40d8a1cd2e77f588a055d28097fc3410d53/skill.md
repo: HatcherLabs/hatcher-skill
kind: skill
stars: 0
last_pushed: 2026-04-20T10:01:51Z
license: mit
score: 9
domains: [agents-ai, backend-api, cli-tools]
tags: [agent-hosting, api-integration, satellite-docs]
curated: 2026-06-16
curated_by: config-scout
---

# HatcherLabs/hatcher-skill — skill

**Why it's worth keeping:** Employs a sophisticated 'satellite file' pattern to manage context window efficiency and includes highly actionable, stateful interaction flows (e.g., email verification polling).

**Summary:** An index file that provides a structured roadmap for managing AI agents on the Hatcher platform via API.

**Source credibility:** Low public social proof (0 stars), but demonstrates professional-grade documentation structure for agentic workflows.

**Recency:** Extremely current; specifically mentions modern Claude Code versions in its telemetry examples.

**Source:** [HatcherLabs/hatcher-skill/skill.md](https://github.com/HatcherLabs/hatcher-skill/blob/d7a6a40d8a1cd2e77f588a055d28097fc3410d53/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: hatcher-skill
version: 1.0.0
description: Deploy and control AI agents on Hatcher (hatcher.host) — managed hosting platform for OpenClaw, Hermes, ElizaOS, and Milady agents.
homepage: https://hatcher.host
api_base: https://api.hatcher.host
---

# Hatcher Skill

Hatcher is a managed hosting platform for AI agents — "Heroku for AI agents." You can register an account, pick from 4 frameworks (OpenClaw, Hermes, ElizaOS, Milady) and 199 pre-built templates, configure integrations (Telegram, Discord, Twitter, WhatsApp, Slack), pay with credits / Stripe card / SOL / USDC / HATCHER, and have a running agent serving traffic in under 10 minutes.

This file is the index. Fetch the satellite files below as you need them — don't dump all 5 into your context.

## Satellite files — fetch as needed

Use the absolute URLs — relative paths resolve to `hatcher.host/<file>.md` which serves the web app, not the markdown.

| File | When to fetch |
| --- | --- |
| [`auth.md`](https://hatcher.host/skill/auth.md) | Registering, email verification polling, creating API keys |
| [`agents.md`](https://hatcher.host/skill/agents.md) | Picking a framework, browsing templates, creating and controlling a
```

</details>
