---
name: POPWorldMedia__POPForums
source: https://github.com/POPWorldMedia/POPForums/blob/8ed15494708aa1cdcc6dad4c63acf48e77738e63/CLAUDE.md
repo: POPWorldMedia/POPForums
kind: claude-md
stars: 206
last_pushed: 2026-06-09T00:53:28Z
license: other
score: 9
domains: [backend-api, web-development, .net]
tags: [aspnet-core, docker, testing, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# POPWorldMedia/POPForums — claude-md

**Why it's worth keeping:** Provides explicit dependency direction logic and DI registration patterns that prevent architectural drift, plus specific command-line filters for granular testing.

**Summary:** A highly detailed guide for a multi-project ASP.NET Core solution covering build/test commands, architecture patterns, and Docker-based local setup.

**Source credibility:** High; active repository with significant GitHub stars and recent maintenance.

**Recency:** Extremely current, targeting .NET 10.

**Source:** [POPWorldMedia/POPForums/CLAUDE.md](https://github.com/POPWorldMedia/POPForums/blob/8ed15494708aa1cdcc6dad4c63acf48e77738e63/CLAUDE.md) · 206★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

POP Forums is an ASP.NET Core forum and Q&A application targeting .NET 10. It uses SignalR for real-time updates, TypeScript for front-end components, and SQL Server as the primary data store.

## Solution Structure

| Project | Purpose |
|---|---|
| `PopForums` | Core business logic, service interfaces, repository interfaces, models |
| `PopForums.Sql` | SQL Server data access implementations, caching layer, migrations scripts |
| `PopForums.Mvc` | ASP.NET MVC area (`/Forums`), controllers, views, TypeScript client, CSS |
| `PopForums.Web` | Host app template — references above projects, contains `Program.cs` |
| `PopForums.AzureKit` | Azure-specific implementations: Redis cache, Azure Search, Blob Storage, queues |
| `PopForums.AzureKit.Functions` | Azure Functions implementations for background jobs |
| `PopForums.ElasticKit` | ElasticSearch search implementation |
| `PopForums.Test` | xUnit tests using NSubstitute, covers services and some MVC code |

## Build Commands

### .NET
```bash
# Build entire solution
dotnet build PopForums.sln

# Ru
```

</details>
