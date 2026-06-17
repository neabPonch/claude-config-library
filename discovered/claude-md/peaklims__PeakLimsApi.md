---
name: peaklims__PeakLimsApi
source: https://github.com/peaklims/PeakLimsApi/blob/37946602864cd3db208a8770d73a2cb8031c316d/CLAUDE.md
repo: peaklims/PeakLimsApi
kind: claude-md
stars: 73
last_pushed: 2026-01-26T18:02:30Z
license: other
score: 9
domains: [.net, backend-api, ddd]
tags: [vertical-slice, cqrs, dotnet-9, mediatr]
curated: 2026-06-15
curated_by: config-scout
---

# peaklims/PeakLimsApi — claude-md

**Why it's worth keeping:** The 'Creating New Features' checklist provides a perfect prescriptive workflow for an agent, and the architectural pattern definitions prevent AI from introducing standard N-tier boilerplate.

**Summary:** Defines a strict vertical-slice architecture for a .NET 9 LIMS application, covering build/test commands and infrastructure orchestration.

**Source credibility:** Strong; shows high professional engineering standards and consistent architectural patterns despite moderate star count.

**Recency:** 

**Source:** [peaklims/PeakLimsApi/CLAUDE.md](https://github.com/peaklims/PeakLimsApi/blob/37946602864cd3db208a8770d73a2cb8031c316d/CLAUDE.md) · 73★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Build and Run
- `dotnet run --project PeakLims/src/PeakLims` - Run the main API
- `dotnet build` - Build the solution
- `docker-compose up --build` - Start infrastructure (databases, Keycloak, Jaeger)

### Database Operations
- `dotnet ef database update --project PeakLims/src/PeakLims` - Apply migrations
- `dotnet ef migrations add <MigrationName> --project PeakLims/src/PeakLims` - Create new migration

### Testing
- `dotnet test` - Run all tests
- `dotnet test PeakLims/tests/PeakLims.UnitTests` - Run unit tests only
- `dotnet test PeakLims/tests/PeakLims.IntegrationTests` - Run integration tests only
- `dotnet test PeakLims/tests/PeakLims.FunctionalTests` - Run functional tests only

### Authentication Setup
Set up Keycloak with Pulumi:
1. `cd PeakLimsIdp`
2. `pulumi login --local`
3. `pulumi up`

## Architecture Overview

This is a **Vertical Slice Architecture .NET 9.0 application** implementing **Domain-Driven Design (DDD)** and **CQRS** patterns for a Laboratory Information Management System (LIMS).

### Key Architectural Patterns
```

</details>
