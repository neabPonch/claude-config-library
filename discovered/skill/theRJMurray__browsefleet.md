---
name: theRJMurray__browsefleet
source: https://github.com/theRJMurray/browsefleet/blob/2118d13cfa07e825d6cc28eb205fc3152f271248/skill.md
repo: theRJMurray/browsefleet
kind: skill
stars: 2
last_pushed: 2026-06-02T04:01:45Z
license: mit
score: 9
domains: [backend-api, web-scraping, automation-agents]
tags: [onboarding, smoke-tests, agent-instructions, node-js]
curated: 2026-06-14
curated_by: config-scout
---

# theRJMurray/browsefleet — skill

**Why it's worth keeping:** The 'Smoke Test' sequence provides a verifiable lifecycle for the agent to confirm service health; the TL;DR block optimizes token usage for startup.

**Summary:** A highly structured agent onboarding guide that includes environment verification through an automated multi-step smoke test.

**Source credibility:** Very recent activity and high-quality technical documentation structure.

**Recency:** Highly current, optimized for modern Node.js environments.

**Source:** [theRJMurray/browsefleet/skill.md](https://github.com/theRJMurray/browsefleet/blob/2118d13cfa07e825d6cc28eb205fc3152f271248/skill.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Working in browsefleet with a coding agent

This file is read by AI coding agents that land in this repo (Claude Code, Cursor, Aider, etc.). It contains the exact setup, run, test, and contribution steps. Read it once at the start of any session; refer back to it on errors. The README points here from its AI Agent banner.

For human contributors, this file is also accurate and useful. There is no separate "human onboarding" doc.

## TL;DR for the impatient agent

```bash
git clone https://github.com/theRJMurray/browsefleet.git
cd browsefleet
cp .env.example .env
npm install
npm run dev
# in another terminal:
curl http://localhost:3000/health
```

Expected last line: `{"status":"ok","version":"0.1.0","activeSessions":0,"maxSessions":30,"uptime":<seconds>}`.

If any of those steps fail, jump to "Known failure modes" at the bottom of this file before trying anything else.

## Required tools and versions

| Tool                        | Minimum                 | Why                                                                                                       |
| --------------------------- | ----------------------- | -----------------------------------------------------------
```

</details>
