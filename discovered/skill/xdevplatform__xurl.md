---
name: xdevplatform__xurl
source: https://github.com/xdevplatform/xurl/blob/b8d4863fba4f0f1a065abbfbdcb2fd011bdf9680/SKILL.md
repo: xdevplatform/xurl
kind: skill
stars: 1106
last_pushed: 2026-05-21T01:13:00Z
license: mit
score: 9
domains: [cli-tools, api-interaction, social-media]
tags: [x-api, automation, security-first]
curated: 2026-06-14
curated_by: config-scout
---

# xdevplatform/xurl — skill

**Why it's worth keeping:** It includes a critical 'Secret Safety' section to prevent credential leakage and uses highly structured documentation (tables + examples) that is optimized for LLM parsing.

**Summary:** A comprehensive skill file for interacting with the X API via the xurl CLI, covering posting, reading, and social graph management.

**Source credibility:** High; the source repo has significant community traction with over 1,100 stars.

**Recency:** Current; reflects modern CLI/API interaction patterns used by contemporary agents.

**Source:** [xdevplatform/xurl/SKILL.md](https://github.com/xdevplatform/xurl/blob/b8d4863fba4f0f1a065abbfbdcb2fd011bdf9680/SKILL.md) · 1106★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: xurl
description: A curl-like CLI tool for making authenticated requests to the X (Twitter) API. Use this skill when you need to post tweets, reply, quote, search, read posts, manage followers, send DMs, upload media, or interact with any X API v2 endpoint. Supports multiple apps, OAuth 2.0, OAuth 1.0a, and app-only auth.
---

# xurl — Agent Skill Reference

`xurl` is a CLI tool for the X API. It supports both **shortcut commands** (human/agent‑friendly one‑liners) and **raw curl‑style** access to any v2 endpoint. All commands return JSON to stdout.

---

## Prerequisites

This skill requires the `xurl` CLI utility: <https://github.com/xdevplatform/xurl>.

Before using any command you must be authenticated. Run `xurl auth status` to check.

### Secret Safety (Mandatory)

- Never read, print, parse, summarize, upload, or send `~/.xurl` (or copies of it) to the LLM context.
- Never ask the user to paste credentials/tokens into chat.
- The user must fill `~/.xurl` with required secrets manually on their own machine.
- Do not recommend or execute auth commands with inline secrets in agent/LLM sessions.
- Warn that using CLI secret options in agent sessions can leak credential
```

</details>
