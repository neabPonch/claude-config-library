---
name: NoMercy-Entertainment__nomercy-media-server
source: https://github.com/NoMercy-Entertainment/nomercy-media-server/blob/b1ca3703a7dd96c9a7ee7d91855ce9b3dc2ed27b/CLAUDE.md
repo: NoMercy-Entertainment/nomercy-media-server
kind: claude-md
stars: 10
last_pushed: 2026-06-13T23:31:13Z
license: other
score: 9
domains: [backend-api, dotnet]
tags: [csharp, .net, coding-standards, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# NoMercy-Entertainment/nomercy-media-server — claude-md

**Why it's worth keeping:** The 'Explicitly avoid' section prevents common LLM mistakes like EF Core translation errors, and the mandatory 'Storage Facade' rule enforces critical architectural seams for filesystem access.

**Summary:** A highly prescriptive guide for C#/.NET development that defines strict coding standards, project structure, and architectural boundaries.

**Source credibility:** The repository is a specialized media server with clear, high-level architecture and recent activity.

**Recency:** Extremely current, referencing .NET 10 and modern C# features like primary constructors and collection expressions.

**Source:** [NoMercy-Entertainment/nomercy-media-server/CLAUDE.md](https://github.com/NoMercy-Entertainment/nomercy-media-server/blob/b1ca3703a7dd96c9a7ee7d91855ce9b3dc2ed27b/CLAUDE.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# NoMercy Media Server

The flagship media server for encoding, organizing, and streaming personal media.

See `.claude/CLAUDE.md` for the full detailed guide (build commands, architecture, security, dev container, etc.)

## Tech Stack
- C# / .NET 10, ASP.NET Core, Entity Framework Core (SQLite)
- SignalR for real-time communication
- MSBuild / dotnet CLI, solution file: `NoMercy.Server.sln`
- Centralized package management: `Directory.Packages.props`
- Testing: xUnit + FluentAssertions + Moq (12 test projects)

## Structure
```
src/
  NoMercy.Service/          # Web host entry point
  NoMercy.Cli/              # CLI entry point
  NoMercy.Launcher/         # Desktop launcher
  NoMercy.Tray/             # System tray (Avalonia)
  NoMercy.App/              # App entry point
  NoMercy.Api/              # Controllers, DTOs, Hubs, Middleware
  NoMercy.Database/         # EF Core models and migrations
  NoMercy.Data/             # Data access layer
  NoMercy.Encoder/          # Media encoding/transcoding
  NoMercy.MediaProcessing/  # Media analysis and processing
  NoMercy.MediaSources/     # Media source providers
  NoMercy.Providers/        # External data providers (TMDB, etc.)
  NoMe
```

</details>
