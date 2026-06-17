---
name: AgOpenGPS-Official__AgValoniaGPS__claude
source: https://github.com/AgOpenGPS-Official/AgValoniaGPS/blob/f7ee84a0d675255bdf5856d5eef4a5ee8b5dcecf/AgOpen_Snapshot/CLAUDE.md
repo: AgOpenGPS-Official/AgValoniaGPS
kind: claude-md
stars: 65
last_pushed: 2026-06-15T16:28:22Z
license: apache-2.0
score: 7
domains: [dotnet, c#]
tags: [build-commands, architecture, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# AgOpenGPS-Official/AgValoniaGPS — claude-md

**Why it's worth keeping:** Demonstrates how to include specific command flags (like --no-restore) and maps out the logical hierarchy of various project components.

**Summary:** Provides detailed build/test commands and architectural patterns for a multi-project .NET solution.

**Source credibility:** High; part of an active, high-star agricultural software project.

**Recency:** Current in format/structure, though content contains legacy tech stack discrepancies relative to the new repository description.

**Source:** [AgOpenGPS-Official/AgValoniaGPS/AgOpen_Snapshot/CLAUDE.md](https://github.com/AgOpenGPS-Official/AgValoniaGPS/blob/f7ee84a0d675255bdf5856d5eef4a5ee8b5dcecf/AgOpen_Snapshot/CLAUDE.md) · 65★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview
AgOpenGPS is a precision agriculture guidance software written in C# (.NET Framework 4.8) that provides GPS guidance, field mapping, and section control for agricultural equipment. The project consists of two main applications: AgIO (communication hub) and AgOpenGPS (main application).

## Build Commands

```bash
# Restore dependencies
dotnet restore --runtime win-x64 ./SourceCode/AgOpenGPS.sln

# Build solution
dotnet build --no-restore ./SourceCode/AgOpenGPS.sln

# Run all tests
dotnet test --no-restore --no-build ./SourceCode/AgOpenGPS.sln

# Run specific test project
dotnet test ./SourceCode/AgLibrary.Tests/AgLibrary.Tests.csproj
dotnet test ./SourceCode/AgOpenGPS.Core.Tests/AgOpenGPS.Core.Tests.csproj

# Publish (creates AgOpenGPS folder with all applications)
dotnet publish ./SourceCode/AgOpenGPS.sln
```

## Architecture

### Core Structure
- **MVP Pattern**: AgOpenGPS.Core implements Model-View-Presenter pattern with dependency injection
- **ApplicationCore**: Main composition root at `AgOpenGPS.Core/ApplicationCore.cs`
- **Separation of Co
```

</details>
