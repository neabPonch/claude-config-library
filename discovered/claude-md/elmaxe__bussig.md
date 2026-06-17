---
name: elmaxe__bussig
source: https://github.com/elmaxe/bussig/blob/d9dbabbf85b83f4405dc337aa5e42464efb2a551/CLAUDE.md
repo: elmaxe/bussig
kind: claude-md
stars: 2
last_pushed: 2026-06-09T18:15:32Z
license: mit
score: 9
domains: [backend, .net, database]
tags: [architecture-diagram, test-patterns, dotnet]
curated: 2026-06-15
curated_by: config-scout
---

# elmaxe/bussig — claude-md

**Why it's worth keeping:** The ASCII layer diagram provides crucial structural context; the inclusion of specific test-filtering syntax avoids AI trial-and-error during verification.

**Summary:** A high-quality guide featuring a visual architectural hierarchy and specific command patterns for testing and formatting.

**Source credibility:** Low star count suggests a niche or new library, but the documentation quality is professional.

**Recency:** Highly current, referencing bleeding-edge .NET 10 and C# 14 standards.

**Source:** [elmaxe/bussig/CLAUDE.md](https://github.com/elmaxe/bussig/blob/d9dbabbf85b83f4405dc337aa5e42464efb2a551/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Bussig is a PostgreSQL-based message bus library for .NET. It provides distributed messaging with queues, dead letter queues, delayed message processing, distributed locks, message scheduling, and large message attachments via the claim check pattern.

## Build & Development Commands

```bash
# Build solution
dotnet build

# Run all tests
dotnet test

# Run specific test project
dotnet run --project src/Bussig.Tests.Unit
dotnet run --project src/Bussig.Tests.Integration

# Run a single test (TUnit uses --filter)
dotnet test --filter "FullyQualifiedName~MessageUrnTests"

# Format code (CSharpier)
dotnet tool restore
dotnet csharpier format .

# Check formatting without modifying
dotnet csharpier check .
```

**Note:** Integration tests require Docker for TestContainers (PostgreSQL).

## Architecture

```
┌──────────────────────────────────────────────────────────┐
│                    Application Layer                     │
│         Uses IBus.SendAsync / ScheduleAsync              │
├──────────────────────────────────────────────────────────┤
│
```

</details>
