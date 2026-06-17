---
name: DotNetLabX__dotnet-microservices
source: https://github.com/DotNetLabX/dotnet-microservices/blob/7c0d344126635653528045ba53788477fec3d5ea/claude.md
repo: DotNetLabX/dotnet-microservices
kind: claude-md
stars: 15
last_pushed: 2026-04-22T21:42:15Z
license: mit
score: 9
domains: [backend-api, dotnet, microservices]
tags: [architecture-guardrails, llm-context-management, ddd, vertical-slice]
curated: 2026-06-15
curated_by: config-scout
---

# DotNetLabX/dotnet-microservices — claude-md

**Why it's worth keeping:** The 'Architecture Guardrails' provide actionable prohibitions to prevent common patterns, while the 'Compaction/File Re-read Rules' are brilliant meta-instructions for managing LLM context efficiency.

**Summary:** A highly structured instruction file that combines deep architectural context with strict behavioral constraints for an LLM. It defines a sophisticated workflow involving custom agents, skill sets, and feature plans.

**Source credibility:** High-quality instructional content likely used for professional training (Udemy).

**Recency:** Very current; includes advanced instructions for agentic workflows and context management.

**Source:** [DotNetLabX/dotnet-microservices/claude.md](https://github.com/DotNetLabX/dotnet-microservices/blob/7c0d344126635653528045ba53788477fec3d5ea/claude.md) · 15★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Articles Application — DotNetLabX

Article lifecycle system: draft → submission → review → production → publish. ArticleHub aggregates latest state across services via integration events. Built for a Udemy course on DDD + Vertical Slice + CQRS, evolving from modular monolith to microservices.

## Repo structure

```
src/
├── BuildingBlocks/
│   ├── Articles.Abstractions        — Shared article interfaces & enums (ArticleStage, IArticleAction, ArticleCommandBase)
│   ├── Articles.Grpc.Contracts      — gRPC code-first contracts ([ServiceContract]/[ProtoContract])
│   ├── Articles.Integration.Contracts — MassTransit integration event records
│   ├── Articles.Security            — JWT config, role constants, authorization handlers
│   ├── Blocks.Core                  — Guards, IClaimsProvider, caching, extensions, RequestContext
│   ├── Blocks.Domain                — Entity<T>, AggregateRoot<T>, ValueObject, IDomainEvent
│   ├── Blocks.EntityFrameworkCore   — ApplicationDbContext, TenantDbContext, design-time factory
│   ├── Blocks.Exceptions            — HttpException hierarchy (BadRequest/NotFound/Unauthorized)
│   ├── Blocks.AspNetCore            — AssignUserIdFilter, HttpContextP
```

</details>
