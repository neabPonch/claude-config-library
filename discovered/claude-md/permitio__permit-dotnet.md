---
name: permitio__permit-dotnet
source: https://github.com/permitio/permit-dotnet/blob/ebac22884a8f0b77c828dcc437b432de59c11439/CLAUDE.md
repo: permitio/permit-dotnet
kind: claude-md
stars: 4
last_pushed: 2025-11-09T12:09:10Z
license: apache-2.0
score: 8
domains: [.net, backend-api, sdk-development]
tags: [dotnet, openapi, architecture]
curated: 2026-06-17
curated_by: config-scout
---

# permitio/permit-dotnet — claude-md

**Why it's worth keeping:** Includes an essential 'Auto-Generated Code' warning to prevent the AI from attempting to edit sensitive files; uses component-based descriptions rather than just directory listing.

**Summary:** Provides comprehensive architectural guidance and command-line workflows for a .NET SDK. It explicitly maps functional roles to specific files and structures.

**Source credibility:** High; originated from a professional production SDK (Permit.io).

**Recency:** Current; references modern .NET frameworks (.NET 8/9).

**Source:** [permitio/permit-dotnet/CLAUDE.md](https://github.com/permitio/permit-dotnet/blob/ebac22884a8f0b77c828dcc437b432de59c11439/CLAUDE.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the Permit.io .NET SDK - a client library for the Permit.io full-stack permissions platform. The SDK enables permission checks, user/role management, and tenant administration through both an API client and Policy Decision Point (PDP) enforcement engine.

## Development Commands

### Building the Solution
```bash
dotnet build Permit.sln
```

### Running Tests
```bash
dotnet test tests/PermitTests/PermitTests.csproj
```

### Running Example Application
```bash
dotnet run --project examples/PermitOnboardingApp/PermitOnboardingApp.csproj
```

### Code Formatting
Code formatting is handled automatically via lint-staged with csharpier:
```bash
dotnet csharpier
```

### OpenAPI Code Generation
To update the auto-generated API client code:
```bash
./generate_openapi.sh
```

This script:
- Downloads OpenAPI schemas from Permit.io APIs
- Transforms union types to simple types via Python script
- Generates C# client code using NSwag
- Fixes status code checks for 204 responses

## Architecture Overview

### Core Components

**Main SDK Class (`src/p
```

</details>
