---
name: s87343472__backlink-pilot__skill
source: https://github.com/s87343472/backlink-pilot/blob/926d9235b34d9c6920f524063feadf09c8fbe355/docs/skill.md
repo: s87343472/backlink-pilot
kind: skill
stars: 301
last_pushed: 2026-03-29T07:05:40Z
license: mit
score: 7
domains: [seo, marketing-automation, cli-tools, web-scraping]
tags: [backlinks, seo, browser-automation, indie-hacker]
curated: 2026-06-15
curated_by: config-scout
---

# s87343472/backlink-pilot — skill

**Why it's worth keeping:** Provides a clear 'Scout -> Submit' two-step agentic workflow and specific instructions on bypassing browser automation walls using the bb-browser engine.

**Summary:** Automates SEO backlink submissions through directory scouting and submission workflows. It intelligently handles anti-bot measures like Cloudflare and OAuth via a specialized browser engine.

**Source credibility:** 301 stars indicates a proven, popular utility within the indie hacker community.

**Recency:** Highly relevant as it addresses modern web challenges like Cloudflare Turnstile and OAuth manual intervention.

**Source:** [s87343472/backlink-pilot/docs/skill.md](https://github.com/s87343472/backlink-pilot/blob/926d9235b34d9c6920f524063feadf09c8fbe355/docs/skill.md) · 301★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: backlink-pilot
description: Use for submitting products to directory sites, awesome-lists, or search engines.
disable-auto-invoke: true
---

# Backlink Pilot

Automated backlink submission for indie products. One config, one command.

## Setup

```bash
cd ~/Downloads/backlink-pilot
cp config.example.yaml config.yaml   # edit with product details
```

### Engine Options

| Engine | Setup | Pros |
|--------|-------|------|
| **playwright** (default) | `npm install` | No extension needed |
| **bb** (recommended) | `npm install -g bb-browser` + Chrome extension | Real browser, no anti-bot, no Cloudflare/OAuth issues |

Set in `config.yaml` → `browser.engine: bb` or use `--engine bb` flag.

## Commands

```bash
node src/cli.js scout <url> --deep              # discover form fields
node src/cli.js submit <site>                   # submit to directory
node src/cli.js submit <site> --engine bb       # use real Chrome
node src/cli.js submit https://any-site.com     # generic submission (bb-browser)
node src/cli.js submit <site> --dry-run         # preview only
node src/cli.js awesome <list-key>              # generate awesome-list issue
node src/cli.js indexnow <url>
```

</details>
