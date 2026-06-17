---
name: banane-io__PDB
source: https://github.com/banane-io/PDB/blob/aeef9a1df9256dcc3e561f82a0bec66d0823182e/CLAUDE.md
repo: banane-io/PDB
kind: claude-md
stars: 3
last_pushed: 2026-04-29T16:28:33Z
license: apache-2.0
score: 8
domains: [backend-api, game-dev, dotnet]
tags: [aspnetcore, ef-core, postgresql, game-logic]
curated: 2026-06-14
curated_by: config-scout
---

# banane-io/PDB — claude-md

**Why it's worth keeping:** It encodes critical business rules like grid dimensions and direction offsets, preventing the AI from hallucinating incorrect movement or map loading logic.

**Summary:** Provides specific build commands, architectural layers, and essential game-world domain logic.

**Source credibility:** Low star count (3), but high-quality documentation for a small specialized project.

**Recency:** Very current, utilizing ASP.NET Core 9 and PostgreSQL 17.

**Source:** [banane-io/PDB/CLAUDE.md](https://github.com/banane-io/PDB/blob/aeef9a1df9256dcc3e561f82a0bec66d0823182e/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
dotnet build                    # Build project
dotnet run                      # Run development server (localhost:5079 HTTP, localhost:7079 HTTPS)
dotnet clean                    # Clean build artifacts
dotnet ef database update       # Apply pending migrations
dotnet ef migrations add <Name> # Create a new migration
docker compose up               # Run app + PostgreSQL via Docker
```

Swagger UI is available at `/swagger` when running in Development mode.

## Architecture

**PDB** is an ASP.NET Core 9 Web API backend for a text-based browser RPG (25×25 grid world). The frontend lives in a separate repository (`pdb-frontend`).

**Stack:** C# / ASP.NET Core 9 / Entity Framework Core 9 / PostgreSQL 17

**Layer structure:**
- `Controllers/` — API endpoints (thin, delegate to services)
- `Services/` — Business logic (e.g., `MapPointService` handles grid loading with 5-cell radius, neighbor calculation via `Direction` offsets)
- `Models/` — Domain entities (`MapPoint`, `Hero`, `Base`) and enums (`Direction`, `Terrain`, `Action`)
- `ApplicationConte
```

</details>
