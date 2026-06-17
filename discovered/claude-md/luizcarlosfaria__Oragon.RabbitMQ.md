---
name: luizcarlosfaria__Oragon.RabbitMQ
source: https://github.com/luizcarlosfaria/Oragon.RabbitMQ/blob/017d8b683698c3df73688ee95d3e5ccdb7082c15/CLAUDE.md
repo: luizcarlosfaria/Oragon.RabbitMQ
kind: claude-md
stars: 86
last_pushed: 2026-06-10T08:04:07Z
license: unknown
score: 9
domains: [backend-api, messaging]
tags: [dotnet, rabbitmq, architecture, integration-testing]
curated: 2026-06-15
curated_by: config-scout
---

# luizcarlosfaria/Oragon.RabbitMQ — claude-md

**Why it's worth keeping:** It provides a clear 'Consumer Pipeline' sequence and 'Registration Flow' code snippets which allow the AI to understand execution order. The inclusion of exact Docker commands for reproducing the local build environment is exceptionally useful for debugging tests.

**Summary:** A high-density technical guide that covers architecture flow, specific build commands, and code examples for library usage.

**Source credibility:** High; a well-maintained repository with significant stars and recent activity.

**Recency:** Extremely current, targeting .NET 9/10 and modern development workflows.

**Source:** [luizcarlosfaria/Oragon.RabbitMQ/CLAUDE.md](https://github.com/luizcarlosfaria/Oragon.RabbitMQ/blob/017d8b683698c3df73688ee95d3e5ccdb7082c15/CLAUDE.md) · 86★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Oragon.RabbitMQ is a Minimal API implementation for consuming RabbitMQ queues in .NET. It provides a fluent configuration API similar to ASP.NET Core's Minimal APIs, with built-in resilience features using RabbitMQ.Client 7.x natively (not HTTP/Kestrel-based).

## Build Commands

```bash
# Build all projects (uses solution XML format)
dotnet build ./Oragon.RabbitMQ.slnx

# Run unit tests (uses xUnit)
dotnet test ./tests/Oragon.RabbitMQ.UnitTests/Oragon.RabbitMQ.UnitTests.csproj

# Run integration tests (requires Docker for Testcontainers.RabbitMq)
dotnet test ./tests/Oragon.RabbitMQ.IntegratedTests/Oragon.RabbitMQ.IntegratedTests.csproj

# Run a single test
dotnet test --filter "FullyQualifiedName~TestMethodName"

# Pack a specific project
dotnet pack ./src/Oragon.RabbitMQ/Oragon.RabbitMQ.csproj --configuration Release -p:PackageVersion=1.0.0
```

## Target Frameworks

Projects target `net9.0` and `net10.0`. The solution uses C# preview language features with nullable enabled by default (disabled in test projects).

## Architecture

### Core Proj
```

</details>
