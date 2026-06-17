---
name: SimonCropp__Delta
source: https://github.com/SimonCropp/Delta/blob/58236ccb7c49457b697cd4b5bffb5d77850a7209/claude.md
repo: SimonCropp/Delta
kind: claude-md
stars: 1511
last_pushed: 2026-06-15T00:29:00Z
license: mit
score: 9
domains: [.net, backend-api]
tags: [architecture, documentation-workflow, testing]
curated: 2026-06-16
curated_by: config-scout
---

# SimonCropp/Delta — claude-md

**Why it's worth keeping:** It includes precise CLI commands for filtered testing and establishes 'golden rules' to prevent the agent from editing generated files instead of source files.

**Summary:** Provides a highly structured map of project architecture and specific instructions for managing auto-generated documentation.

**Source credibility:** Strong; high star count and active maintenance on a specialized .NET library.

**Recency:** Current; references modern .NET versions (8/9/10) and specific tool behaviors.

**Source:** [SimonCropp/Delta/claude.md](https://github.com/SimonCropp/Delta/blob/58236ccb7c49457b697cd4b5bffb5d77850a7209/claude.md) · 1511★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Delta is a .NET library that implements HTTP 304 Not Modified responses using database change tracking. It generates ETags from `{AssemblyWriteTime}-{DbTimeStamp}-{OptionalSuffix}` to enable browser caching. Published as three NuGet packages: Delta (core), Delta.EF (Entity Framework), Delta.SqlServer.

## Build & Test

```bash
dotnet build src
dotnet test src

# Run a single test
dotnet test src/DeltaTests --filter "FullyQualifiedName~TestName"
dotnet test src/Delta.EFTests --filter "FullyQualifiedName~TestName"
```

Requires .NET SDK 10.0.103 (preview), pinned in `src/global.json`.

## Architecture

Three library projects under `src/`:

- **Delta/** — Core middleware (`UseDelta()`) for raw `DbConnection`. Handles ETag calculation, cache headers, and 304 responses. Targets net8.0/net9.0/net10.0.
- **Delta.EF/** — Entity Framework wrapper (`UseDelta<TDbContext>()`). Targets net10.0 only.
- **Delta.SqlServer/** — SQL Server-specific change tracking queries. Targets net8.0/net9.0/net10.0.

Key source files:
- `DeltaExtensions_Middleware.cs` — Reques
```

</details>
