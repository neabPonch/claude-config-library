---
name: aj-geddes__useful-ai-prompts__skill
source: https://github.com/aj-geddes/useful-ai-prompts/blob/3f5182cfd739fc113f4af5244a1cf342ad7f7911/skills/rate-limiting-implementation/SKILL.md
repo: aj-geddes/useful-ai-prompts
kind: skill
stars: 267
last_pushed: 2026-03-04T08:20:59Z
license: mit
score: 8
domains: [backend-api, security, distributed-systems]
tags: [rate-limiting, algorithms, architecture, api-design]
curated: 2026-06-16
curated_by: config-scout
---

# aj-geddes/useful-ai-prompts — skill

**Why it's worth keeping:** Provides specific algorithmic patterns (Token Bucket vs Sliding Window) alongside critical production guardrails like cost-based limiting and distributed state management via Redis.

**Summary:** A comprehensive architectural blueprint for implementing rate-limiting, throttling, and API protection mechanisms.

**Source credibility:** 267 stars indicates a well-regarded community curation of AI prompting resources.

**Recency:** Highly relevant; these architectural patterns are fundamental to modern backend engineering.

**Source:** [aj-geddes/useful-ai-prompts/skills/rate-limiting-implementation/SKILL.md](https://github.com/aj-geddes/useful-ai-prompts/blob/3f5182cfd739fc113f4af5244a1cf342ad7f7911/skills/rate-limiting-implementation/SKILL.md) · 267★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: rate-limiting-implementation
description: >
  Implement rate limiting, throttling, API quotas, and backpressure mechanisms
  to protect services from abuse and ensure fair resource usage. Use when
  building APIs, preventing DOS attacks, or managing system load.
---

# Rate Limiting Implementation

## Table of Contents

- [Overview](#overview)
- [When to Use](#when-to-use)
- [Quick Start](#quick-start)
- [Reference Guides](#reference-guides)
- [Best Practices](#best-practices)

## Overview

Implement rate limiting and throttling mechanisms to protect your services from abuse, ensure fair resource allocation, and maintain system stability under load.

## When to Use

- Protecting public APIs from abuse
- Preventing DOS/DDOS attacks
- Ensuring fair resource usage across users
- Implementing API quotas and billing tiers
- Managing system load and backpressure
- Enforcing SLA limits
- Controlling third-party API usage
- Database connection management

## Quick Start

Minimal working example:

```typescript
interface TokenBucketConfig {
  capacity: number;
  refillRate: number; // tokens per second
  refillInterval: number; // milliseconds
}

class TokenBucket {
  private toke
```

</details>
