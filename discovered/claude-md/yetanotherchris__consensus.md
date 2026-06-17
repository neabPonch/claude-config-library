---
name: yetanotherchris__consensus
source: https://github.com/yetanotherchris/consensus/blob/c4bef57b34aa43c70a56cf407d41db9f5fb7c84b/CLAUDE.md
repo: yetanotherchris/consensus
kind: claude-md
stars: 0
last_pushed: 2026-06-14T00:35:35Z
license: unknown
score: 9
domains: [backend-api, ai-agents, cli-tools]
tags: [clean-architecture, dotnet-9, solid-principles]
curated: 2026-06-14
curated_by: config-scout
---

# yetanotherchris/consensus — claude-md

**Why it's worth keeping:** It provides actionable 'how-to' steps for extending the codebase (e.g., DI registration workflows) and strict rules for dependency management via Central Package Management to prevent version drift.

**Summary:** A highly detailed technical manual covering project hierarchy, execution commands, and specific architectural patterns for a .NET-based AI orchestration system.

**Source credibility:** Individual developer project with zero stars, but exhibits professional-grade structural documentation.

**Recency:** Extremely current; uses .NET 9.0 and modern development paradigms.

**Source:** [yetanotherchris/consensus/CLAUDE.md](https://github.com/yetanotherchris/consensus/blob/c4bef57b34aa43c70a56cf407d41db9f5fb7c84b/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Consensus is a .NET 9.0 application that queries multiple AI models with the same prompt and synthesizes a consensus answer. It supports both CLI and web API modes with a React frontend.

## Project Structure

The solution follows a clean architecture with SOLID principles:

- **Consensus.Core** - Core business logic and services (shared library)
- **Consensus.Console** - CLI application for standalone execution
- **Consensus.Api** - ASP.NET Core Web API with Quartz.NET job scheduling
- **Consensus.Web** - React + TypeScript + Vite frontend with Tailwind CSS
- **Consensus.RedisTest** - Redis integration testing utilities

### Key Components

#### Consensus.Core Architecture

- **ConsensusOrchestrator** - Main orchestration of the parallel-then-synthesize workflow
- **Services/** - Service layer implementing SOLID principles:
  - `IAgentService` / `AgentService` - AI agent initialization and queries
  - `IPromptBuilder` / `PromptBuilder` - Prompt construction for different scenarios
  - `ISynthesizerService` / `SynthesizerService` - Synthesizes re
```

</details>
