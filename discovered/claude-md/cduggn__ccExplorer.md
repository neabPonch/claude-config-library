---
name: cduggn__ccExplorer
source: https://github.com/cduggn/ccExplorer/blob/ad73b2fe20200cd1b93a6a89a98903c8fff5e5c0/CLAUDE.md
repo: cduggn/ccExplorer
kind: claude-md
stars: 47
last_pushed: 2026-01-27T23:04:12Z
license: mit
score: 8
domains: [cli-tools, cloud-infrastructure]
tags: [golang, architecture, aws, design-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# cduggn/ccExplorer — claude-md

**Why it's worth keeping:** It explicitly maps data flow and design patterns (Strategy, Adapter), which ensures the AI follows specific structural constraints rather than just writing functional code.

**Summary:** Provides a comprehensive architectural mental model alongside essential build and test commands.

**Source credibility:** A real-world cloud tool with moderate engagement/stars suggesting a professional structure.

**Recency:** Very recent (5 months ago) and perfectly aligned with current Claude Code context requirements.

**Source:** [cduggn/ccExplorer/CLAUDE.md](https://github.com/cduggn/ccExplorer/blob/ad73b2fe20200cd1b93a6a89a98903c8fff5e5c0/CLAUDE.md) · 47★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

**Build and Test:**
- `make build` - Build application to bin/ directory
- `make test` - Run all tests
- `make test-race` - Run tests with race detection
- `make test-cover` - Run tests with coverage
- `make lint` - Run golangci-lint
- `make run` - Run application directly

**Release:**
- `make release` - Create release using goreleaser

## Architecture Overview

ccExplorer is a CLI tool for AWS cost analysis that follows clean architecture patterns with clear separation of concerns.

**Core Data Flow:**
1. CLI layer (`cmd/cli/`) parses commands and flags using Cobra
2. Commands synthesize requests to internal domain types (`internal/types/`)
3. AWS service layer (`internal/awsservice/`) calls Cost Explorer API
4. Utils (`internal/utils/`) transform AWS responses to internal types
5. Writer layer (`internal/writer/`) formats output (stdout, CSV, charts, Pinecone vector DB)

**Key Architectural Patterns:**
- **Dependency Inversion**: Interfaces defined in `internal/ports/` 
- **Factory Pattern**: Writer creation based on output format in `inte
```

</details>
