---
name: nanotaboada__Dotnet.Samples.AspNetCore.WebApi
source: https://github.com/nanotaboada/Dotnet.Samples.AspNetCore.WebApi/blob/fc497a305cda09047b8cb40546c095b09457a7f6/CLAUDE.md
repo: nanotaboada/Dotnet.Samples.AspNetCore.WebApi
kind: claude-md
stars: 9
last_pushed: 2026-06-16T00:54:32Z
license: mit
score: 9
domains: [backend-api, .net]
tags: [aspnet-core, testing-patterns, architecture-rules]
curated: 2026-06-16
curated_by: config-scout
---

# nanotaboada/Dotnet.Samples.AspNetCore.WebApi — claude-md

**Why it's worth keeping:** The inclusion of the 'Mocking validators' section provides a critical technical gotcha regarding FluentValidation/Moq interaction, which prevents common AI-generated bugs. The rigid test naming tables and tree structure also ensure architectural consistency.

**Summary:** A highly structured guide for an ASP.NET Core 10 API that covers architecture, tech stack, and strict testing protocols. It includes specific instructions on how to handle dependency injection and error patterns.

**Source credibility:** High; the project uses cutting-edge .NET 10 and follows modern enterprise patterns.

**Recency:** Extremely current, targeting the latest .NET ecosystem.

**Source:** [nanotaboada/Dotnet.Samples.AspNetCore.WebApi/CLAUDE.md](https://github.com/nanotaboada/Dotnet.Samples.AspNetCore.WebApi/blob/fc497a305cda09047b8cb40546c095b09457a7f6/CLAUDE.md) · 9★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Claude Code

- Run `/pre-commit` to execute the full pre-commit checklist for this project.

## Overview

REST API for managing football players built with ASP.NET Core 10. Implements CRUD operations with a layered architecture, EF Core persistence (SQLite by default, PostgreSQL opt-in via `DATABASE_PROVIDER`), FluentValidation, AutoMapper, and in-memory caching. Primarily a learning and reference project — clarity and educational value take precedence over brevity.

## Tech Stack

| Category        | Technology                                                |
|-----------------|-----------------------------------------------------------|
| Language        | C# (.NET 10 LTS)                                         |
| Framework       | ASP.NET Core (MVC controllers)                           |
| ORM             | Entity Framework Core 10                                  |
| Database        | SQLite (default) · PostgreSQL 17 (opt-in)                |
| Mapping         | AutoMapper                                                |
| Validation      | FluentValidation                                          |
| Caching         | `IMemoryCache` (10-min sliding + 1-hour
```

</details>
