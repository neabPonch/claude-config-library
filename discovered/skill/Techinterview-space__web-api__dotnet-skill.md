---
name: Techinterview-space__web-api__dotnet-skill
source: https://github.com/Techinterview-space/web-api/blob/d23309c965e8c70f7cb697363c82c9d7870b72d5/dotnet-skill.md
repo: Techinterview-space/web-api
kind: skill
stars: 2
last_pushed: 2026-06-05T04:51:12Z
license: gpl-3.0
score: 8
domains: [backend-api, .net]
tags: [clean-architecture, cqrs-lite, mediator-pattern, aspnetcore]
curated: 2026-06-14
curated_by: config-scout
---

# Techinterview-space/web-api — skill

**Why it's worth keeping:** Contains highly transferable code snippets for assembly scanning and service provider extensions that ensure structural consistency across features without heavy dependencies.

**Summary:** Defines a specific Clean Architecture implementation using a lightweight, custom CQRS-lite mediator pattern for .NET.

**Source credibility:** High technical density; appears to be extracted from an actual working production system rather than a tutorial.

**Recency:** Highly current, utilizing modern C# record types and pattern matching.

**Source:** [Techinterview-space/web-api/dotnet-skill.md](https://github.com/Techinterview-space/web-api/blob/d23309c965e8c70f7cb697363c82c9d7870b72d5/dotnet-skill.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# .NET Backend Best Practices Skill

Use this before writing any .NET backend code, before planning code changes and enhancements. This establishes style guidelines, architecture patterns, and teaches essential .NET techniques derived from a production-grade Clean Architecture project.

---

## Architecture

### Clean Architecture Layers

```
Web.Api (Presentation Layer)
  - Controllers, Features, Middlewares, Setup
  - References: Infrastructure, Domain
    ↓
Infrastructure (Infrastructure Layer)
  - Database (EF Core), External Services, AI, Email, Storage
  - References: Domain
    ↓
Domain (Core Layer)
  - Entities, Value Objects, Enums, Validation
  - References: Nothing (zero external dependencies)
```

**Rules:**
- Domain MUST NOT reference Infrastructure or Web.Api
- Infrastructure MUST NOT reference Web.Api
- Web.Api references both Infrastructure and Domain
- Keep Domain free from framework dependencies (no EF Core, no ASP.NET)

### Solution Structure

```
src/
├── Web.Api/                    # ASP.NET Core API host
│   ├── Features/               # Feature-based organization (controllers + handlers)
│   ├── Middlewares/             # HTTP pipeline middlewares
│   ├── Set
```

</details>
