---
name: suphero__fixit
source: https://github.com/suphero/fixit/blob/e997eb34d1a5068c40312debc46d23afd716aa37/Claude.md
repo: suphero/fixit
kind: claude-md
stars: 0
last_pushed: 2026-03-10T08:12:34Z
license: unknown
score: 9
domains: [web-frontend, ecommerce, fullstack]
tags: [remix, shopify, typescript, prisma]
curated: 2026-06-16
curated_by: config-scout
---

# suphero/fixit — claude-md

**Why it's worth keeping:** The 'Key Conventions' section provides exact code patterns to prevent common framework errors, and the 'DO/DON'T' list includes excellent meta-instructions for agent behavior like avoiding unnecessary abstractions.

**Summary:** Provides highly specific architectural constraints and tech stack versions for a Remix/Shopify application.

**Source credibility:** Low social proof (0 stars), but the content reflects a professional, high-context production environment.

**Recency:** Current; uses modern Remix v2 and contemporary Shopify integration patterns.

**Source:** [suphero/fixit/Claude.md](https://github.com/suphero/fixit/blob/e997eb34d1a5068c40312debc46d23afd716aa37/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Guidelines for Smart Forecast

This document provides guidelines for using Claude Code effectively with the Smart Forecast Shopify app.

## Project Overview

Smart Forecast is a Shopify app built with Remix that provides product recommendations and impact tracking for merchants. The app helps merchants make data-driven decisions about their inventory and product offerings.

## Tech Stack

- **Framework**: [Remix](https://remix.run) v2.7.1
- **Runtime**: Node.js v18.20+ / v20.10+ / v21.0.0+
- **Language**: TypeScript 5.2.2
- **Database**: Prisma ORM with SQLite (production should use PostgreSQL/MySQL)
- **Shopify Integration**:
  - `@shopify/shopify-app-remix` v3.4.0
  - `@shopify/app-bridge-react` v4.1.6
  - `@shopify/polaris` v12.0.0
- **UI**: Polaris design system
- **Message Queue**: RabbitMQ (amqplib)

## Project Structure

```
smart-forecast/
├── app/
│   ├── routes/              # Remix routes (file-based routing)
│   ├── models/              # Data models and business logic
│   │   ├── *.server.ts      # Server-side only code
│   │   └── *.business.server.ts # Business logic layer
│   ├── utils/               # Utility functions
│   ├── constants/           # A
```

</details>
