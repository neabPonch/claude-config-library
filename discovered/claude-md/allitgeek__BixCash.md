---
name: allitgeek__BixCash
source: https://github.com/allitgeek/BixCash/blob/a94b9fc2284fa0b0b689e75ec0ed5cbda5bd9732/claude.md
repo: allitgeek/BixCash
kind: claude-md
stars: 0
last_pushed: 2026-04-23T20:50:34Z
license: unknown
score: 7
domains: [backend-api, web-development]
tags: [technical-journal, api-documentation, database-schema]
curated: 2026-06-15
curated_by: config-scout
---

# allitgeek/BixCash — claude-md

**Why it's worth keeping:** The inclusion of structured API endpoint specifications and database schema changes provides immediate context for an agent to build or debug without manual exploration.

**Summary:** A high-density technical journal and documentation file that tracks project architecture, API definitions, and recent development milestones.

**Source credibility:** Low star count; likely a single developer's personal project documentation.

**Recency:** Highly current, referencing bleeding-edge/future technologies like Laravel 12.

**Source:** [allitgeek/BixCash/claude.md](https://github.com/allitgeek/BixCash/blob/a94b9fc2284fa0b0b689e75ec0ed5cbda5bd9732/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# BixCash Development Documentation

**Last Updated**: October 17, 2025
**Project**: BixCash - Shop to Earn Platform
**Environment**: Production (bixcash.com)
**Server**: GCP (34.55.43.43)

---

## Project Overview

BixCash is a cashback rewards platform where customers earn rewards by shopping with partner brands. The platform consists of:
- **Customer App**: Mobile-first web app for customers to browse brands, make purchases, and earn cashback
- **Partner Portal**: Interface for brands to manage their offers and promotions
- **Admin Panel**: Backend management system for platform administration

---

## Technology Stack

### Backend
- **Framework**: Laravel 12
- **PHP**: 8.3
- **Database**: MySQL (bixcash_prod)
- **Authentication**: Laravel Sanctum (API tokens)
- **Queue**: Database driver with Supervisor (2 workers)
- **Scheduler**: Laravel Cron (runs every minute)

### Frontend
- **Build Tool**: Vite
- **CSS**: Custom CSS with CSS variables
- **JavaScript**: Vanilla JS (no framework)

### Infrastructure
- **Web Server**: Apache 2.4 with mod_php
- **SSL**: Let's Encrypt (auto-renewing)
- **Process Manager**: Supervisor for queue workers
- **Domain**: bixcash.com (via Namecheap D
```

</details>
