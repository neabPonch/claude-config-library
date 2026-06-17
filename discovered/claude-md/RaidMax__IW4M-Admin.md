---
name: RaidMax__IW4M-Admin
source: https://github.com/RaidMax/IW4M-Admin/blob/e33fc98b182b50d066cf248a443b9f97b71c9e61/CLAUDE.md
repo: RaidMax/IW4M-Admin
kind: claude-md
stars: 249
last_pushed: 2026-06-14T20:25:17Z
license: mit
score: 9
domains: [backend-api, dotnet, game-server]
tags: [dotnet, multi-database, plugin-system, fullstack]
curated: 2026-06-15
curated_by: config-scout
---

# RaidMax/IW4M-Admin — claude-md

**Why it's worth keeping:** It captures critical 'tribal knowledge' regarding the dual-generation plugin system and the necessity of manual multi-provider migrations, while providing a clear dependency graph.

**Summary:** A highly detailed technical guide covering multi-stage build processes for both backend and frontend, alongside complex database migration requirements.

**Source credibility:** High; well-starred repository with active maintenance and recent commits.

**Recency:** Highly current, referencing cutting-edge technologies like .NET 10.0 and EF Core 9.0.

**Source:** [RaidMax/IW4M-Admin/CLAUDE.md](https://github.com/RaidMax/IW4M-Admin/blob/e33fc98b182b50d066cf248a443b9f97b71c9e61/CLAUDE.md) · 249★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What is IW4MAdmin

IW4MAdmin is a game server administration tool for Call of Duty dedicated servers (IW4x, IW6x, Pluto T6/IW5, CoD4x, TeknoMW3, etc.). It monitors server activity, manages players (bans/kicks/warnings), tracks stats, and provides a web interface for administration.

## Build Commands

```bash
# Restore packages
dotnet restore IW4MAdmin.sln

# Build the full solution (Debug)
dotnet build IW4MAdmin.sln

# Build the main application
dotnet build Application/Application.csproj

# Build a specific plugin
dotnet build Plugins/Stats/Stats.csproj

# Publish the application (Prerelease config used in CI)
dotnet publish Application/Application.csproj -c Prerelease -o Publish/Prerelease

# Build all plugins (from repo root)
find Plugins -name "*.csproj" -exec dotnet publish {} -c Debug -o BUILD/Plugins \;
```

Build configurations: `Debug`, `Release`, `Prerelease`. Target framework: `net10.0`.

In Debug mode, a PreBuild PowerShell script runs and `PluginDebugReference` is included (it aggregates all plugin projects for easier debugging).

## Frontend Build
```

</details>
