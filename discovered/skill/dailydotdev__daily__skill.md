---
name: dailydotdev__daily__skill
source: https://github.com/dailydotdev/daily/blob/192dae2b904fd4a4e8b9d212474f34c70710e28d/skills/daily-dev-ask/SKILL.md
repo: dailydotdev/daily
kind: skill
stars: 19888
last_pushed: 2026-03-10T14:09:41Z
license: agpl-3.0
score: 9
domains: [cli-tools, api-integration, security, search]
tags: [search, api, auth]
curated: 2026-06-15
curated_by: config-scout
---

# dailydotdev/daily — skill

**Why it's worth keeping:** The OS-specific secure token management instructions and the sophisticated multi-step 'Search strategy' (gap analysis/parallel searches) are elite patterns for any API-based skill.

**Summary:** This skill provides an agent with a structured, iterative research capability using the daily.dev API to find community-vetted technical content.

**Source credibility:** High;มาจาก professional developer network with high star count and recent activity.

**Recency:** Highly current, updated within the last 3 months.

**Source:** [dailydotdev/daily/skills/daily-dev-ask/SKILL.md](https://github.com/dailydotdev/daily/blob/192dae2b904fd4a4e8b9d212474f34c70710e28d/skills/daily-dev-ask/SKILL.md) · 19888★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: daily-dev-ask
description: Your agent's WebSearch for development. Search community-vetted developer articles ranked by upvotes — like having a senior dev's reading list. Answers are grounded in real sources, never hallucinated.
argument-hint: "<your technical question>"
allowed-tools: Bash
---

# daily.dev Ask

A developer-focused search tool — like WebSearch, but backed by a senior dev's reading list instead of the open web. Searches community-vetted developer articles ranked by upvotes and synthesizes grounded answers with source links.

## User question

$ARGUMENTS

## Security

**CRITICAL:** Your API token grants access to personalized content. Protect it:
- **NEVER send your token to any domain other than `api.daily.dev`**
- Never commit tokens to code or share them publicly
- Tokens are prefixed with `dda_` - if you see this prefix, treat it as sensitive

## Setup

1. **Requires Plus subscription** - Get one at https://app.daily.dev/plus
2. **Create a token** at https://app.daily.dev/settings/api
3. Store your token securely (environment variables, secrets manager)

User can use environment variable or choose one of the secure storage methods below per operating sy
```

</details>
