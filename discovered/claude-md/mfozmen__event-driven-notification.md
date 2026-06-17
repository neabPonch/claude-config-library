---
name: mfozmen__event-driven-notification
source: https://github.com/mfozmen/event-driven-notification/blob/b58b5e53cb02558be02241cbbd58763bb1e1b90f/CLAUDE.md
repo: mfozmen/event-driven-notification
kind: claude-md
stars: 0
last_pushed: 2026-03-14T20:14:01Z
license: unknown
score: 9
domains: [backend-api, php-laravel]
tags: [tdd, workflow-control, testing-rigor, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# mfozmen/event-driven-notification — claude-md

**Why it's worth keeping:** The 'Pause for user commit' pattern prevents messy git histories during agentic development, while the specific edge-case testing instructions mitigate AI logic gaps.

**Summary:** This file establishes rigorous TDD/testing requirements and a strict step-by-step execution workflow that forces the agent to pause for user review and commits.

**Source credibility:** Low star count/single developer, but displays high-level professional engineering standards.

**Recency:** Highly current; utilizes Laravel 11 and Pest 3.

**Source:** [mfozmen/event-driven-notification/CLAUDE.md](https://github.com/mfozmen/event-driven-notification/blob/b58b5e53cb02558be02241cbbd58763bb1e1b90f/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Event-Driven Notification System for Insider One — a scalable REST API that processes and delivers messages through SMS, Email, and Push channels. Handles high throughput, reliable delivery with retries, and real-time status tracking.

## Tech Stack

- **Framework**: PHP Laravel 11
- **Queue / Cache / Rate Limiting**: Redis
- **Database**: MySQL 8
- **Containerization**: Docker Compose (one-command setup, all env vars in docker-compose.yml)
- **API Docs**: Swagger/OpenAPI via L5-Swagger
- **Testing**: Pest 3 (TDD — tests first, then implement)
- **Code Quality**: Laravel Pint, PHPStan (Larastan level 6)
- **External Provider**: webhook.site (simulates SMS/Email/Push delivery)

## Development Approach

**Test-Driven Development (TDD)** — write tests first, run them (they fail), then implement to make them pass.

## Testing Rules

Every phase must include BOTH unit tests and feature tests. Unit tests cover isolated logic (services, DTOs, enums, strategies, value objects). Feature tests cover HTTP endpoints and full request lifecycle. Never skip unit tests —
```

</details>
