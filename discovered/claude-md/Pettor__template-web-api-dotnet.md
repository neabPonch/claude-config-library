---
name: Pettor__template-web-api-dotnet
source: https://github.com/Pettor/template-web-api-dotnet/blob/10110eabe123c816bca90df5554c99c218c1f31c/CLAUDE.md
repo: Pettor/template-web-api-dotnet
kind: claude-md
stars: 2
last_pushed: 2026-06-13T21:08:23Z
license: mit
score: 9
domains: [backend-api, .net]
tags: [clean-architecture, cqrs, dotnet, web-api]
curated: 2026-06-16
curated_by: config-scout
---

# Pettor/template-web-api-dotnet — claude-md

**Why it's worth keeping:** Explicit layer dependency rules and the detailed CQRS pattern blueprint prevent AI from breaking architecture; 'What Not To Do' section provides excellent negative constraints.

**Summary:** Provides strict architectural guardrails and structural patterns for a .NET Clean Architecture web API.

**Source credibility:** High-quality, engineered template despite low star count.

**Recency:** Extremely current, targeting .NET 10.0 and C# 14.

**Source:** [Pettor/template-web-api-dotnet/CLAUDE.md](https://github.com/Pettor/template-web-api-dotnet/blob/10110eabe123c816bca90df5554c99c218c1f31c/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — AI Assistant Guide

This document provides guidance for AI assistants (Claude and others) working in this repository. It covers codebase structure, development workflows, and conventions to follow.

## Project Overview

This is a **production-ready, enterprise-grade .NET 10.0 Web API template** implementing Clean Architecture with multitenancy support. It is designed as a reusable starting point for scalable, maintainable web API services.

**Repository:** `pettor/template-web-api-dotnet`

---

## Architecture

The project follows **Clean Architecture** with four clearly separated layers:

```
src/
├── Core/
│   ├── Domain/           # Entities, value objects, domain events — no external deps
│   ├── Application/      # CQRS handlers, DTOs, validators, use cases
│   └── Shared/           # Shared contracts and interfaces
├── Infrastructure/       # EF Core, Auth, Caching, Mailing, Hangfire, etc.
├── Host/                 # ASP.NET Core entry point: controllers, middleware, config
└── Migrators/
    └── Migrators.PostgreSQL/  # EF Core migrations for PostgreSQL
tests/
└── Infrastructure.Test/  # xUnit unit tests
```

### Layer Dependency Rules

- **Domain** has zero ex
```

</details>
