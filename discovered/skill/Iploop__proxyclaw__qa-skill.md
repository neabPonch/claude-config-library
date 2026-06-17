---
name: Iploop__proxyclaw__qa-skill
source: https://github.com/Iploop/proxyclaw/blob/62d7508cd1030be85bc0866c7360d5ff7e4eb2f9/qa-SKILL.md
repo: Iploop/proxyclaw
kind: skill
stars: 8
last_pushed: 2026-04-30T16:48:48Z
license: mit
score: 8
domains: [web-scraping, automation, devops]
tags: [proxy, scraper, anti-bot, qa]
curated: 2026-06-14
curated_by: config-scout
---

# Iploop/proxyclaw — skill

**Why it's worth keeping:** The 'Tiered Strategy' (API vs Proxy vs Scrapling) offers a transferable decision tree for complex scraping, and the 'Known Limitations' section prevents futile tool attempts.

**Summary:** Provides a tiered web scraping strategy using IPLoop proxies and Scrapling anti-bot bypass across 66 sites. It categorizes websites by technical difficulty to guide the agent's approach.

**Source credibility:** Moderate; 8 stars and active updates within the last two months indicate a live project.

**Recency:** Current; shows recent version history and up-to-date site status.

**Source:** [Iploop/proxyclaw/qa-SKILL.md](https://github.com/Iploop/proxyclaw/blob/62d7508cd1030be85bc0866c7360d5ff7e4eb2f9/qa-SKILL.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: iploop-qa-scraper
description: QA web scraping skill using IPLoop proxy infrastructure. Scrapes 66 major sites via SDK v1.5.3 with API extractors, anti-bot bypass, smart fallbacks, and real data extraction. 100% success rate. Use when testing proxy quality, scraping sites through IPLoop, or validating proxy data extraction. Triggers on proxy QA, site scraping, data extraction testing, anti-bot bypass.
---

# IPLoop QA Scraper

Scrape 66 major sites through IPLoop residential proxy + Scrapling anti-bot fingerprinting.

**SDK Version:** v1.8.1 | **Legacy QA Success Rate:** 100% (66/66) | **Install:** `pip install iploop-sdk`

## Strategy: Combo by Default

All sites use Scrapling anti-bot + residential proxy combo. Falls back to plain HTTP if Scrapling fails.

| Tier | Method | Count | Sites |
|------|--------|-------|-------|
| 1 | Public APIs | 12 | YouTube, Stocks, CoinGecko, Spotify, NPM, PyPI, XKCD, ExchangeRate, SpaceX, Pokemon, Weather, RemoteOK |
| 2 | HTTP + Proxy | 28 | Amazon, eBay, TikTok, Target, Airbnb, Cloudflare, Shopify, IMDb, Wikipedia, HackerNews, GitHub, StackOverflow, Steam, Goodreads, Archive.org, CNN, Trustpilot, Craigslist, Newegg, BBC, Medium, DuckD
```

</details>
