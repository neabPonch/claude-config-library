---
name: duyet__monorepo__claude
source: https://github.com/duyet/monorepo/blob/2188c9a5de1bfe360c6f09dab194f2d34f6c6b70/apps/insights/CLAUDE.md
repo: duyet/monorepo
kind: claude-md
stars: 23
last_pushed: 2026-06-15T06:28:30Z
license: mit
score: 9
domains: [web-frontend, data-analytics, react]
tags: [architecture-map, data-flow, pattern-guide]
curated: 2026-06-15
curated_by: config-scout
---

# duyet/monorepo — claude-md

**Why it's worth keeping:** The inclusion of a 'Hybrid Data Architecture' explanation provides critical mental models for complex data merging, while the 'Feature Modules' section gives explicit directory-to-function mapping.

**Summary:** A highly detailed architectural guide for an analytics dashboard that maps out specific feature modules and data-flow logic.

**Source credibility:** High; demonstrates a high degree of technical specificity and clear project structure.

**Recency:** Very current, referencing React 19 and modern development workflows.

**Source:** [duyet/monorepo/apps/insights/CLAUDE.md](https://github.com/duyet/monorepo/blob/2188c9a5de1bfe360c6f09dab194f2d34f6c6b70/apps/insights/CLAUDE.md) · 23★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Insights App Development Guide

This file provides guidance to Claude Code (claude.ai/code) when working with the insights analytics dashboard application.

## Application Overview

The **insights** app is a comprehensive analytics dashboard that aggregates data from multiple sources to provide insights into development productivity, AI usage, and system performance. Built as a Vite SPA with data fetched at build time for optimal performance.

**Live URL**: https://insights.duyet.net | https://duyet-insights.vercel.app

## Architecture & Tech Stack

### Core Technologies

- **Framework**: Vite + TanStack Router (SPA, file-based routing) with React 19
- **Styling**: Tailwind CSS with custom design system
- **Charts**: Recharts with shadcn/ui components
- **Database**: ClickHouse for analytics data
- **Type Safety**: TypeScript with strict mode

### Data Sources Integration

- **GitHub**: Repository statistics, commit activity, language trends
- **PostHog**: User behavior and product analytics
- **WakaTime**: Coding time tracking and productivity metrics
- **Cloudflare**: Website performance and traffic analytics
- **CCUsage**: Claude Code usage and cost analytics (Clic
```

</details>
