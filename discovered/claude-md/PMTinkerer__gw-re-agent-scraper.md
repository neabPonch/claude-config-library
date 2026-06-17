---
name: PMTinkerer__gw-re-agent-scraper
source: https://github.com/PMTinkerer/gw-re-agent-scraper/blob/97530ddf254d57b4de24a252eda2990bb9c8f52d/CLAUDE.md
repo: PMTinkerer/gw-re-agent-scraper
kind: claude-md
stars: 0
last_pushed: 2026-06-14T13:16:11Z
license: unknown
score: 9
domains: [web-scraping, data-engineering, python]
tags: [scraping, automation, operational-knowledge]
curated: 2026-06-15
curated_by: config-scout
---

# PMTinkerer/gw-re-agent-scraper — claude-md

**Why it's worth keeping:** It documents fragile operational constraints like rate limits, proxy rotation strategies, and specific DOM/NUXT field 'gotchas' that prevent an AI from introducing breaking changes to delicate scrapers.

**Summary:** This file serves as a high-density technical manual for complex, multi-stage web scraping pipelines and data enrichment processes.

**Source credibility:** The extreme specificity of technical failure modes and data-schema nuances suggests a highly detailed real-world project.

**Recency:** Very recent; contains verified data observations dated April 2026.

**Source:** [PMTinkerer/gw-re-agent-scraper/CLAUDE.md](https://github.com/PMTinkerer/gw-re-agent-scraper/blob/97530ddf254d57b4de24a252eda2990bb9c8f52d/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Project Does
Scrapes publicly visible sold property data from Redfin for 10 southern coastal Maine towns, then enriches each transaction with listing agent and brokerage data by visiting individual Redfin property pages via Playwright. The primary deliverables are `data/dashboard.html` (HTML leaderboard with trend badges, hosted on GitHub Pages) and `data/agent_leaderboard.md` (markdown version). Runs on GitHub Actions free tier with resumable chunk-based processing.

## Current State (as of 2026-04-16)
- **Maine Listings (MREIS MLS) — PRIMARY source**: 16,024 closed transactions enriched with both listing AND buyer agent across 10 towns, 15-year history (2011-2026). 99.97% enrichment success. Authoritative MLS data. 2,253 unique listing agents, 2,634 unique buyer agents, 3,165 total in search index.
- **Redfin pipeline — ARCHIVED 2026-04-16**: 2,397 transactions captured before retirement. Strictly a subset of Maine MLS (CSV cap, listing-side only, 3-year window). 4x/day cron disabled. Manual dispatch still available in `.github/workflows/scrape_agents.
```

</details>
