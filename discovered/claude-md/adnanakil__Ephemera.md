---
name: adnanakil__Ephemera
source: https://github.com/adnanakil/Ephemera/blob/b6de23e1c6bf7450ae488bb27e1778295f6586f5/claude.md
repo: adnanakil/Ephemera
kind: claude-md
stars: 0
last_pushed: 2026-04-05T21:55:43Z
license: unknown
score: 8
domains: [web-scraping, backend-api, cli-tools]
tags: [scraper, workflow-driven]
curated: 2026-06-16
curated_by: config-scout
---

# adnanakil/Ephemera — claude-md

**Why it's worth keeping:** The 'Custom Tools' section is an excellent pattern that teaches the agent exactly how to use existing scripts with clear examples; the 'Development Workflow' provides high-quality, multi-step procedural knowledge.

**Summary:** Provides highly detailed instructions for using custom CLI tools and a structured workflow for adding new data sources. It also includes critical operational constraints like rate limits and cost warnings.

**Source credibility:** Low social proof (0 stars) but contains highly specific technical instructions consistent with a real-world production environment.

**Recency:** Very recent (2 months ago), aligning with modern Claude Code usage patterns.

**Source:** [adnanakil/Ephemera/claude.md](https://github.com/adnanakil/Ephemera/blob/b6de23e1c6bf7450ae488bb27e1778295f6586f5/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Development Guide - Ephemera NYC

This document contains information for Claude Code to help with development on this project.

## Project Overview

Ephemera is an NYC events aggregation app that scrapes venues across Manhattan, Brooklyn, and Queens. It uses:
- **Next.js** (frontend & API routes)
- **Heroku** (production deployment)
- **Upstash Redis** (event caching)
- **BullMQ** (background job processing)
- **Firecrawl/Scrapfly** (web scraping)
- **Claude Haiku 4.5** (event extraction from HTML)
- **Swift iOS app** (native mobile client)

## Custom Tools

### Venue Scraper Tool

**Location:** `tools/scrape-venue.js`

A Node.js script that uses Scrapfly API to analyze venue websites and find event calendar pages.

**Purpose:**
- Quickly discover event/calendar URLs on venue websites
- Extract relevant links and text mentions
- Test if venues are scrapable before adding them to the main scraper

**Setup:**
```bash
# API key is stored in .env.local
SCRAPFLY_API_KEY=scp-live-0f7f4cd9f9f9462782dfaadcd93cfa40
```

**Usage:**
```bash
# Basic usage with default search terms (event|calendar|show)
node tools/scrape-venue.js <url>

# Custom search term
node tools/scrape-venue.js <
```

</details>
