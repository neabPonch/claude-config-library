---
name: jamesprsudderth__Car
source: https://github.com/jamesprsudderth/Car/blob/7528ba7098b376333130ce97e5b2a6fd89e29b64/CLAUDE.MD
repo: jamesprsudderth/Car
kind: claude-md
stars: 0
last_pushed: 2026-02-06T01:03:06Z
license: unknown
score: 8
domains: [web-scraping, nextjs, backend-api]
tags: [scraper, puppeteer, prisma, nextjs]
curated: 2026-06-15
curated_by: config-scout
---

# jamesprsudderth/Car — claude-md

**Why it's worth keeping:** The 'Notes for Claude' section provides high-value guardrails (Prisma singleton usage, live data caution) that prevent common AI coding errors in this specific stack.

**Summary:** A comprehensive project blueprint for a Next.js/Puppeteer car scraper that outlines system architecture, database schemas, and specific scraping workflows.

**Source credibility:** Low-signal source (0 stars), but the documentation structure is professional and highly useful.

**Recency:** Current; utilizes Next.js 14 and modern TypeScript patterns.

**Source:** [jamesprsudderth/Car/CLAUDE.MD](https://github.com/jamesprsudderth/Car/blob/7528ba7098b376333130ce97e5b2a6fd89e29b64/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AutoFind NYC - Car Inventory Scraper

## Project Overview

AutoFind NYC is a Next.js application that scrapes car inventory data from multiple dealers and provides an AI-powered search interface. The system automatically collects, stores, and updates car listings from various sources.

## Technology Stack

- **Framework**: Next.js 14 (App Router)
- **Language**: TypeScript
- **Database**: PostgreSQL with Prisma ORM
- **Styling**: Tailwind CSS
- **Web Scraping**: Puppeteer (headless browser automation)
- **AI**: OpenAI API for natural language search
- **Scheduling**: node-cron for automated scraping

## Architecture

### Database Schema (Prisma)

**Dealer Model**
- Stores dealer information (name, website, scrape configuration)
- Tracks scraping status and schedule
- Related to cars and scrape logs

**Car Model**
- Vehicle listings with detailed specs (brand, model, year, price, mileage, etc.)
- Tracked over time (firstSeen, lastSeen, isActive)
- Supports multiple images
- Indexed for efficient search (brand, price, year, mileage, condition, vehicleType)

**ScrapeLog Model**
- Audit trail of scraping operations
- Tracks success/failure, duration, and counts

### Key Directories
```

</details>
