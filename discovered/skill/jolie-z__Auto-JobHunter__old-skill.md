---
name: jolie-z__Auto-JobHunter__old-skill
source: https://github.com/jolie-z/Auto-JobHunter/blob/4f9dec38978035a87d34cab5b15914dc8688e6f0/boss_scraper/old_SKILL.md
repo: jolie-z/Auto-JobHunter
kind: skill
stars: 41
last_pushed: 2026-04-27T02:16:38Z
license: other
score: 9
domains: [cli-tools, automation, agents-ai]
tags: [job-search, recruitment, china]
curated: 2026-06-17
curated_by: config-scout
---

# jolie-z/Auto-JobHunter — skill

**Why it's worth keeping:** Includes sophisticated authentication state-machine logic and critical anti-detection/rate-limiting guidelines essential for safe automated behavior.

**Summary:** Provides a comprehensive interface for interacting with the BOSS Zhipin job platform via CLI, covering job searches, profile management, and applications.

**Source credibility:** Niche specialized tool with steady maintenance.

**Recency:** Very recent (last pushed 2 months ago).

**Source:** [jolie-z/Auto-JobHunter/boss_scraper/old_SKILL.md](https://github.com/jolie-z/Auto-JobHunter/blob/4f9dec38978035a87d34cab5b15914dc8688e6f0/boss_scraper/old_SKILL.md) · 41★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: boss-cli
description: Use boss-cli for ALL BOSS 直聘 operations — searching jobs, viewing recommendations, managing applications, chatting with recruiters, and batch greeting. Invoke whenever the user requests any job search or recruitment platform interaction on BOSS 直聘.
author: jackwener
version: "0.3.0"
tags:
  - boss
  - zhipin
  - boss直聘
  - job-search
  - recruitment
  - cli
---

# boss-cli — BOSS 直聘 CLI Tool

**Binary:** `boss`
**Credentials:** browser cookies (auto-extracted from 10+ browsers) or QR code login (`--qrcode`)

## Setup

```bash
# Install (requires Python 3.10+)
uv tool install kabi-boss-cli
# Or: pipx install kabi-boss-cli

# Upgrade to latest (recommended)
uv tool upgrade kabi-boss-cli
# Or: pipx upgrade kabi-boss-cli
```

## Authentication

**IMPORTANT FOR AGENTS**: Before executing ANY boss command, check if credentials exist first. Do NOT assume cookies are configured.

### Step 0: Check if already authenticated

```bash
boss status --json 2>/dev/null | jq -r '.authenticated' | grep -q true && echo "AUTH_OK" || echo "AUTH_NEEDED"
```

If `AUTH_OK`, skip to [Command Reference](#command-reference).
If `AUTH_NEEDED`, proceed to Step 1.

### Step 1: Gu
```

</details>
