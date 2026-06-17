---
name: upstash__ratelimit-js__skill
source: https://github.com/upstash/ratelimit-js/blob/5b5448a5f0bae809cd624a7c639771a8b2e227cb/skills/SKILL.md
repo: upstash/ratelimit-js
kind: skill
stars: 2038
last_pushed: 2026-03-09T11:38:46Z
license: mit
score: 7
domains: [backend-api, security]
tags: [rate-limiting, typescript, redis]
curated: 2026-06-15
curated_by: config-scout
---

# upstash/ratelimit-js — skill

**Why it's worth keeping:** The quick-start example includes exact dependency imports and class instantiations to prevent API hallucination. The links to specific sub-docs allow an agent to efficiently navigate from basic setup to advanced algorithm tuning.

**Summary:** Provides a concise integration pattern for the Upstash Redis Rate Limit SDK.

**Source credibility:** High; Upstash is a well-established provider in the serverless ecosystem with significant community traction.

**Recency:** Current; maintained within the last 3 months.

**Source:** [upstash/ratelimit-js/skills/SKILL.md](https://github.com/upstash/ratelimit-js/blob/5b5448a5f0bae809cd624a7c639771a8b2e227cb/skills/SKILL.md) · 2038★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: upstash-ratelimit-ts
description: Lightweight guidance for using the Redis Rate Limit TypeScript SDK, including setup steps, basic usage, and pointers to advanced algorithm, features, pricing, and traffic‑protection docs.
---

# Rate Limit TS SDK

## Quick Start
- Install the SDK and connect to Redis.
- Create a rate limiter and apply it to incoming operations.

Example:
```ts
import { Ratelimit } from "@upstash/ratelimit";
import { Redis } from "@upstash/redis";

const redis = new Redis({ url: "<url>", token: "<token>" });
const limiter = new Ratelimit({ redis, limiter: Ratelimit.slidingWindow(5, "10s") });

const { success } = await limiter.limit("user-id");
if (!success) {
  // throttled
}
```

## Other Skill Files
- **algorithms.md**: Describes all available rate‑limiting algorithms and how they behave.
- **pricing-cost.md**: Explains pricing, Redis cost implications, and operational considerations.
- **features.md**: Lists SDK features such as prefixes, custom keys, and behavioral options.
- **methods-getting-started.md**: Full method reference for the SDK's API and getting started guide.
- **traffic-protection.md**: Guidance on applying rate limiting for traffic sha
```

</details>
