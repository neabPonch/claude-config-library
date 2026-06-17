---
name: johnlokerse__azure-devops-bicep-local-deploy
source: https://github.com/johnlokerse/azure-devops-bicep-local-deploy/blob/696706511a577f2ba935d6f9867e59f48318143f/CLAUDE.MD
repo: johnlokerse/azure-devops-bicep-local-deploy
kind: claude-md
stars: 37
last_pushed: 2026-05-24T13:32:20Z
license: unknown
score: 9
domains: [cli-tools, infrastructure-as-code, backend-api]
tags: [csharp, bicep, azure, architecture-patterns]
curated: 2026-06-14
curated_by: config-scout
---

# johnlokerse/azure-devops-bicep-local-deploy — claude-md

**Why it's worth keeping:** Uses 'Reference Implementations' to guide the LLM toward existing patterns and includes explicit prohibitions against common shorthand/abbreviations to ensure code quality.

**Summary:** Provides architectural blueprints, detailed handler development patterns, and strict coding standards for a C#/.NET 9 extension.

**Source credibility:** A specialized project with recent activity (1 month ago) using modern .NET 9 stack.

**Recency:** Highly current; explicitly integrates Claude Code tool usage patterns like 'subagent_type=Explore'.

**Source:** [johnlokerse/azure-devops-bicep-local-deploy/CLAUDE.MD](https://github.com/johnlokerse/azure-devops-bicep-local-deploy/blob/696706511a577f2ba935d6f9867e59f48318143f/CLAUDE.MD) · 37★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.MD

This file provides context and instructions specifically for Claude Code when working on the Azure DevOps Bicep Local-Deploy extension.

## Project Overview

This is an **experimental** Azure Bicep local-deploy extension that configures Azure DevOps via its REST API. The extension allows users to define Azure DevOps resources (projects, repositories, artifact feeds, service connections, permissions, extensions, work items, and pipeline runs) in Bicep templates and deploy them locally.

**Primary languages:**
- **C# (.NET 9)** for the extension implementation
- **Bicep** for usage samples and templates

**Architecture:** Screaming architecture with feature-based folders (e.g., `src/Project/`, `src/Repository/`, `src/ArtifactFeed/`)

**Key documentation:**
- Azure Bicep local-deploy framework: https://techcommunity.microsoft.com/blog/azuregovernanceandmanagementblog/create-your-own-bicep-local-extension-using-net/4439967
- Create your own custom extension for Azure Bicep: https://johnlokerse.dev/2025/10/20/create-your-own-custom-extension-for-azure-bicep/
- C# coding conventions: https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions
```

</details>
