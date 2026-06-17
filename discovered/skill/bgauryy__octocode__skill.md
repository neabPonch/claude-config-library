---
name: bgauryy__octocode__skill
source: https://github.com/bgauryy/octocode/blob/40716767093fc40a4a8a73c47ff64eb2e57a92c9/skills/octocode-news/SKILL.md
repo: bgauryy/octocode
kind: skill
stars: 864
last_pushed: 2026-06-06T23:50:15Z
license: mit
score: 9
domains: [ai, dev-tools, web-platform, security]
tags: [orchestration, research, data-extraction, parallel-agents]
curated: 2026-06-15
curated_by: config-scout
---

# bgauryy/octocode — skill

**Why it's worth keeping:** It demonstrates elite orchestration techniques like the 'resume protocol' for crash recovery, strict schema enforcement between subagents, and delegating heavy data fetching to specialized CLI scripts.

**Summary:** A highly structured research agent that uses a coordinator-subagent architecture to parallelize news discovery across multiple domains and output validated JSON/HTML reports.

**Source credibility:** High; repository shows strong community interest (864 stars) and very recent maintenance.

**Recency:** 

**Source:** [bgauryy/octocode/skills/octocode-news/SKILL.md](https://github.com/bgauryy/octocode/blob/40716767093fc40a4a8a73c47ff64eb2e57a92c9/skills/octocode-news/SKILL.md) · 864★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: octocode-news
description: Researches what is new in AI, developer tools, web platform, security, and notable repositories. Use when the user asks for whats-new, latest updates, recent releases, tech news, AI news, changelogs, repo updates, or trend scanning.
---

# What's New — Tech Research Agent

**Goal**: Lock scope, sweep RSS + cataloged sources in parallel, research gaps, assemble a validated JSON report and an HTML report, then open the HTML in the default browser.

## Quick Input

Use defaults silently when the user did not provide a value. Only ask if the request is genuinely ambiguous.

1. **Domains**: A=AI, B=DevTools, C=Web/JS, D=Security, E=Repos. Default: all
2. **Window**: `24h` / `7d` / `14d` / `30d`. Default: `7d`
3. **Depth**: `brief` / `deep` / `comprehensive`. Default: `deep`

## Non-Negotiables

1. Run both discovery scripts before manual browsing.
2. Treat `references/sources.md` as the baseline catalog, not a suggestion.
3. Use official/product/project sources first; secondary sources validate or widen coverage.
4. Read the full canonical page before writing a kept item summary. RSS snippets are discovery-only.
5. When a source is a daily digest hub
```

</details>
