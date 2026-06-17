---
name: SimonCropp__GraphQL.EntityFramework
source: https://github.com/SimonCropp/GraphQL.EntityFramework/blob/25a607b1fcb168a6577073004c1e3b1f4eeb09f3/claude.md
repo: SimonCropp/GraphQL.EntityFramework
kind: claude-md
stars: 395
last_pushed: 2026-06-15T02:57:13Z
license: mit
score: 9
domains: [backend, .net]
tags: [.net, graphql, architecture-map]
curated: 2026-06-15
curated_by: config-scout
---

# SimonCropp/GraphQL.EntityFramework — claude-md

**Why it's worth keeping:** It includes 'Key Patterns' for idiomatic usage and explicit warnings about auto-generated files to prevent the LLM from making useless edits.

**Summary:** Provides a comprehensive structural map of a .NET library alongside specific build, test, and documentation generation commands.

**Source credibility:** High; 395 stars and very recent activity indicate a stable, well-regarded project.

**Recency:** Current; provides excellent context for modern agentic workflows like Claude Code.

**Source:** [SimonCropp/GraphQL.EntityFramework/claude.md](https://github.com/SimonCropp/GraphQL.EntityFramework/blob/25a607b1fcb168a6577073004c1e3b1f4eeb09f3/claude.md) · 395★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Workflow Guidelines

**IMPORTANT - Git Commits:**
- NEVER automatically commit changes
- NEVER prompt or ask to commit changes
- NEVER suggest creating commits
- The user will handle all git commits manually

## Project Overview

GraphQL.EntityFramework is a .NET library that adds EntityFramework Core IQueryable support to GraphQL.NET. It enables automatic query generation, filtering, pagination, and ordering for GraphQL queries backed by EF Core.

## Build and Test Commands

### Building
```bash
dotnet build src --configuration Release
```

### Running Tests
```bash
# Run all tests except integration tests
dotnet test src --configuration Release --no-build --no-restore --filter Category!=Integration

# Run all tests including integration tests
dotnet test src --configuration Release --no-build --no-restore
```

### Running a Single Test
```bash
# Run a specific test by fully qualified name
dotnet test src --filter "FullyQualifiedName~TestNamespace.TestClass.TestMethod"

# Run all tests in a class
dotnet test src --filter "FullyQualifiedName~TestNamespace.TestClas
```

</details>
