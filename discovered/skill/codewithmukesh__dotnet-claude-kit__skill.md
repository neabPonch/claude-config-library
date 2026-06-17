---
name: codewithmukesh__dotnet-claude-kit__skill
source: https://github.com/codewithmukesh/dotnet-claude-kit/blob/9a9a91107596b3ac3ad1d0ad5ec5eef189e74515/skills/resilience/SKILL.md
repo: codewithmukesh/dotnet-claude-kit
kind: skill
stars: 451
last_pushed: 2026-06-11T20:20:15Z
license: mit
score: 9
domains: [backend, dotnet, cloud-infrastructure]
tags: [resilience, polly, dotnet, reliability, http]
curated: 2026-06-15
curated_by: config-scout
---

# codewithmukesh/dotnet-claude-kit — skill

**Why it's worth keeping:** It enforces modern architectural principles like the 'v8 vs v7' distinction and specifies exact strategy ordering (total timeout > retry > circuit breaker). The inclusion of hedging and OpenTelemetry integration makes it production-ready rather than just a snippet collection.

**Summary:** Provides expert-level implementation patterns for Polly v8 resilience pipelines in .NET. It covers HTTP client defaults, custom DI registration via keyed services, hedging, and telemetry.

**Source credibility:** High; highly rated repository focused on high-performance .NET patterns.

**Recency:** Extremely current, targeting the latest .NET 10 and Polly v8 standards.

**Source:** [codewithmukesh/dotnet-claude-kit/skills/resilience/SKILL.md](https://github.com/codewithmukesh/dotnet-claude-kit/blob/9a9a91107596b3ac3ad1d0ad5ec5eef189e74515/skills/resilience/SKILL.md) · 451★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: resilience
description: >
  Resilience patterns for .NET 10 applications using Polly v8.
  Covers retry, circuit breaker, timeout, fallback, rate limiter, hedging,
  and composing resilience pipelines.
  Load this skill when implementing retry logic, circuit breakers, handling
  transient failures, or when the user mentions "Polly", "resilience",
  "retry", "circuit breaker", "timeout", "fallback", "rate limit",
  "hedging", "transient fault", "HttpClient resilience", or "resilience pipeline".
---

# Resilience

## Core Principles

1. **Polly v8 resilience pipelines, not v7 policies** — Polly v8 replaced `Policy` with `ResiliencePipeline`. Never use `PolicyBuilder`, `Policy.Handle<>()`, or `ISyncPolicy`. The new API is composable, type-safe, and integrates natively with `IHttpClientFactory`.
2. **Configure via `AddResilienceHandler`, not manual wrapping** — For HTTP calls, use `Microsoft.Extensions.Http.Resilience` which adds pipelines directly to `HttpClient` via DI. No manual `ExecuteAsync` wrapping.
3. **Compose strategies, don't nest them** — A single `ResiliencePipeline` can chain retry + circuit breaker + timeout. Strategies execute outer-to-inner (first added = out
```

</details>
