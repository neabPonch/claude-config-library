---
name: ravendb__ravendb
source: https://github.com/ravendb/ravendb/blob/4f37176d134871146773a84997b1276b00b20b84/CLAUDE.md
repo: ravendb/ravendb
kind: claude-md
stars: 3959
last_pushed: 2026-06-15T07:34:22Z
license: other
score: 10
domains: [backend, database-engine, .net, typescript]
tags: [.net, nosql, testing-patterns, architecture-map]
curated: 2026-06-15
curated_by: config-scout
---

# ravendb/ravendb — claude-md

**Why it's worth keeping:** Extremely specific instructions on custom test attributes/base classes to prevent CI failures and detailed tables mapping source code to functional subsystems.

**Summary:** A masterclass in technical documentation that provides deep semantic context for a complex database engine including build, test, and architectural hierarchies.

**Source credibility:** High; RavenDB is a major, production-grade ACID database with high star count and active maintenance.

**Recency:** Highly current, referencing .NET 10 and Node.js 20 LTS.

**Source:** [ravendb/ravendb/CLAUDE.md](https://github.com/ravendb/ravendb/blob/4f37176d134871146773a84997b1276b00b20b84/CLAUDE.md) · 3959★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

RavenDB is an ACID-compliant NoSQL document database. C# (.NET 10) server and client, TypeScript/React web Studio UI. Licensed under AGPLv3.

## Prerequisites

- .NET SDK 10.0.201 (exact version in `global.json`, uses `rollForward: latestFeature`)
- Node.js >= 20.0.0 LTS (for Studio)
- PowerShell (for release builds)

## Build Commands

```bash
# .NET build (server + client, ~5 min) - use this for most work
dotnet build RavenDB.sln -c Release

# Studio initial setup
cd src/Raven.Studio && npm ci && npm run restore_compile

# Studio development (watch mode)
cd src/Raven.Studio && npm run webpack-watch

# Full release build (20+ min, rarely needed)
./build.ps1 -LinuxX64                  # Windows
./build.sh -LinuxX64                   # Linux/Mac
./build.ps1 -JustStudio               # Studio only
./build.ps1 -LinuxX64 -DontRebuildStudio  # Skip Studio rebuild
```

## Testing

```bash
# Fast tests (2-5 min) - primary validation, run frequently
cd test/FastTests && dotnet test --configuration Release

# Run a single test class
dotnet test test/Fa
```

</details>
