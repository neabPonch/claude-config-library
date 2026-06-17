---
name: fsprojects__Paket
source: https://github.com/fsprojects/Paket/blob/3b63da856fa6d6f441d43b9dc2aa64e6ad10fe62/CLAUDE.md
repo: fsprojects/Paket
kind: claude-md
stars: 2083
last_pushed: 2026-01-20T08:53:10Z
license: mit
score: 9
domains: [cli-tools, dotnet, fsharp]
tags: [architecture, build-automation, testing-patterns]
curated: 2026-06-14
curated_by: config-scout
---

# fsprojects/Paket — claude-md

**Why it's worth keeping:** The structured breakdown of logical architectural layers and the specific, filter-able test commands are highly transferable techniques for helping an AI navigate complex codebases.

**Summary:** Provides comprehensive technical context including build automation, testing patterns, architectural layers, and conditional compilation symbols.

**Source credibility:** High; originates from a well-established F# project within the fsprojects organization.

**Recency:** Current; includes references to modern .NET versions like net9.

**Source:** [fsprojects/Paket/CLAUDE.md](https://github.com/fsprojects/Paket/blob/3b63da856fa6d6f441d43b9dc2aa64e6ad10fe62/CLAUDE.md) · 2083★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Paket is a dependency manager for .NET with support for NuGet packages and git repositories. It maintains transitive dependency information in `paket.lock` alongside `paket.dependencies`, providing explicit control over dependency resolution that NuGet traditionally lacked.

## Build Commands

```bash
# Full build (restores, builds, runs tests)
build.cmd                    # Windows
./build.sh                   # Linux/Mac

# Build with specific targets
build.cmd Build              # Build only
build.cmd QuickTest          # Run unit tests without full build
build.cmd RunTests           # Run all unit tests
build.cmd QuickIntegrationTests  # Run quick integration tests (scriptgen category)
build.cmd RunIntegrationTestsNet # Run full .NET Framework integration tests
build.cmd RunIntegrationTestsNetCore # Run full .NET Core integration tests

# Skip specific stages
build.cmd SkipTests          # Skip all tests
build.cmd SkipIntegrationTests # Skip integration tests only
```

## Testing

**Unit Tests:**
```bash
dotnet test tests/Paket.Tests/Paket.Te
```

</details>
