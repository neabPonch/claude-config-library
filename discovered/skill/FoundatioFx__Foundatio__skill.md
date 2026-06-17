---
name: FoundatioFx__Foundatio__skill
source: https://github.com/FoundatioFx/Foundatio/blob/b793b2e0460bef5f3081a359af32dcd9f001682c/.agents/skills/foundatio/SKILL.md
repo: FoundatioFx/Foundatio
kind: skill
stars: 2088
last_pushed: 2026-06-12T23:09:25Z
license: apache-2.0
score: 9
domains: [.net, backend-api, distributed-systems]
tags: [.net, infrastructure, patterns, dependency-injection]
curated: 2026-06-15
curated_by: config-scout
---

# FoundatioFx/Foundatio — skill

**Why it's worth keeping:** It includes a proactive 'query-docs' instruction using MCP to ensure the agent can fetch fresh API details, avoiding documentation rot. It also provides dense, high-value code patterns that transition easily from local in-memory dev setups to production providers.

**Summary:** Provides comprehensive technical coverage for Foundatio's .NET infrastructure abstractions, including caching, messaging, and distributed jobs.

**Source credibility:** Foundatio is a highly-starred, mature open-source library for distributed .NET application foundations.

**Recency:** Very current; utilizes modern MCP tool-calling strategies intended for agentic workflows.

**Source:** [FoundatioFx/Foundatio/.agents/skills/foundatio/SKILL.md](https://github.com/FoundatioFx/Foundatio/blob/b793b2e0460bef5f3081a359af32dcd9f001682c/.agents/skills/foundatio/SKILL.md) · 2088★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: foundatio
description: >
  Use when working with Foundatio infrastructure abstractions for .NET -- caching,
  queuing, messaging, file storage, distributed locking, or background jobs. Apply
  when using ICacheClient, IQueue, IMessageBus, IFileStorage, ILockProvider, IJob,
  or resilience patterns like retry and circuit breakers. Covers in-memory and
  production implementations (Redis, Azure, AWS, Kafka, RabbitMQ). Use context7
  MCP to fetch current API docs and examples.
---

# Foundatio

Pluggable infrastructure abstractions for distributed .NET apps. Interface-first, testable, swappable between in-memory (dev/test) and production providers (Redis, Azure, AWS) with zero application code changes.

## Documentation via context7

Use context7 MCP for complete, up-to-date API docs and examples. The main library ID covers all abstractions and implementations:

```text
query-docs(libraryId="/foundatiofx/foundatio", query="How to configure queue retry policies and dead letter handling")
```

Query with specific questions, not single keywords. All provider docs (Redis, Azure, AWS, Kafka, etc.) are included in the main library.

## Core Interfaces

| Interface | Purpose | In-M
```

</details>
