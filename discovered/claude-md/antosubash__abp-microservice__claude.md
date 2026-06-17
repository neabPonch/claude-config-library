---
name: antosubash__abp-microservice__claude
source: https://github.com/antosubash/abp-microservice/blob/60faee0c96884fa8ac6049d7781b8fe9f29f2e6d/src/CLAUDE.md
repo: antosubash/abp-microservice
kind: claude-md
stars: 132
last_pushed: 2026-05-31T19:33:14Z
license: mit
score: 9
domains: [backend, microservices, .net]
tags: [makefile-driven, ddd, dotnet-aspire, microservices]
curated: 2026-06-15
curated_by: config-scout
---

# antosubash/abp-microservice — claude-md

**Why it's worth keeping:** It maps a complex multi-service structure to a unified Makefile/command set and provides architectural hierarchy that helps the AI navigate large-scale DDD projects.

**Summary:** A high-density development manual covering orchestration via .NET Aspire, database lifecycle management, and automated code quality workflows.

**Source credibility:** Strong; the repo is well-starred and actively maintained with cutting-edge .NET versions.

**Recency:** Extremely current, utilizing modern .NET 10 and Aspire patterns.

**Source:** [antosubash/abp-microservice/src/CLAUDE.md](https://github.com/antosubash/abp-microservice/blob/60faee0c96884fa8ac6049d7781b8fe9f29f2e6d/src/CLAUDE.md) · 132★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an ABP Framework-based microservices template using .NET Aspire for orchestration. The solution demonstrates a production-grade microservices architecture with four core services (Administration, Identity, Projects, SaaS), a YARP-based API gateway, OpenIddict authentication server, and Blazor WebAssembly frontend.

**Current ABP Version:** 10.0
**Target Framework:** .NET 10.0
**.NET Aspire Version:** 9.5.2

## Quick Start with Makefile

A comprehensive Makefile is available at the repository root for common development tasks:

```bash
# First-time setup
make install          # Restore tools and install git hooks

# Daily workflow
make build            # Build the solution
make test             # Run all tests
make format           # Format code with CSharpier
make fix              # Auto-fix analyzers + style + format
make run              # Run with .NET Aspire orchestration

# Database operations
make migrate          # Run database migrations
make reset-db         # Reset databases (dev only - DESTRUCTIVE)

# Individual services
make r
```

</details>
