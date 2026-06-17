---
name: pdevito3__craftsman
source: https://github.com/pdevito3/craftsman/blob/2a242a06e4a7ae32f76ce9d1a91f8eb342ad6486/CLAUDE.md
repo: pdevito3/craftsman
kind: claude-md
stars: 1172
last_pushed: 2025-10-11T19:08:21Z
license: mit
score: 9
domains: [cli-tools, backend-api]
tags: [dotnet, architecture, scaffolding, mediatr]
curated: 2026-06-14
curated_by: config-scout
---

# pdevito3/craftsman — claude-md

**Why it's worth keeping:** The 'Conventions' section uses concrete code examples to teach the AI exactly how to implement MediatR handlers and use specific string literal markers.

**Summary:** Provides deep architectural context and strict implementation patterns for a complex scaffolding tool.

**Source credibility:** High; a popular .NET project with significant GitHub traction and clear, organized documentation.

**Recency:** Current; demonstrates modern .NET patterns highly compatible with Claude Code's capabilities.

**Source:** [pdevito3/craftsman/CLAUDE.md](https://github.com/pdevito3/craftsman/blob/2a242a06e4a7ae32f76ce9d1a91f8eb342ad6486/CLAUDE.md) · 1172★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

### Build Commands
```bash
dotnet restore                          # Restore dependencies
dotnet build                           # Build the project
dotnet build --configuration Release   # Build for release
dotnet pack                            # Package as NuGet tool
```

### Running the Tool
```bash
dotnet run                             # Run the craftsman tool
craftsman new example MyProject       # Generate example project (when installed globally)
```

### Installation
```bash
dotnet tool install -g craftsman       # Install as global tool
```

## Architecture Overview

Craftsman is a .NET 8 scaffolding tool that generates clean architecture .NET Web APIs. The codebase follows a command-pattern architecture using Spectre.Console.Cli for the CLI interface.

### Core Architecture Components

**Commands** (`/Commands/`): CLI command implementations
- `NewDomainCommand` - Scaffolds complete domain projects
- `NewExampleCommand` - Generates example projects via CLI prompts
- `AddEntityCommand` - Adds entities to existing projects
- `AddFeatureCommand`
```

</details>
