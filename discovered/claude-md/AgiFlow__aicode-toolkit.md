---
name: AgiFlow__aicode-toolkit
source: https://github.com/AgiFlow/aicode-toolkit/blob/f038e632257619907da7aa35e6b1aa8dfd00673c/CLAUDE.md
repo: AgiFlow/aicode-toolkit
kind: claude-md
stars: 159
last_pushed: 2026-06-13T01:23:07Z
license: agpl-3.0
score: 9
domains: [agents-ai, cli-tools, monorepo]
tags: [mcp, workflow-automation, architecture-enforcement]
curated: 2026-06-14
curated_by: config-scout
---

# AgiFlow/aicode-toolkit — claude-md

**Why it's worth keeping:** The 'discovery' pattern is excellent: instead of hardcoding rules in CLAUDE.md, it instructs the agent to use an MCP tool to fetch current standards, ensuring documentation stays fresh and tools stay consistent.

**Summary:** It defines a strict, tool-driven workflow that mandates retrieving design patterns via MCP before editing and running automated reviews after changes. This creates a self-correcting development loop driven by the project's architecture.

**Source credibility:** Highly credible; actively maintained toolkit specializing in AI coding infrastructure.

**Recency:** Very current; optimized for modern MCP-centric workflows used by Claude Code.

**Source:** [AgiFlow/aicode-toolkit/CLAUDE.md](https://github.com/AgiFlow/aicode-toolkit/blob/f038e632257619907da7aa35e6b1aa8dfd00673c/CLAUDE.md) · 159★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code when working with this repository.

## Project Overview

An Nx monorepo for building MCP (Model Context Protocol) servers and tooling. Uses pnpm for package management and Nx for build orchestration.

## Coding Workflow (IMPORTANT)

When working on code in this repository, **ALWAYS** follow this workflow using MCP tools:

### 1. Creating New Applications or Features

**Use scaffold-mcp MCP tools to generate boilerplate code:**

- **List available boilerplates**: Use `list-boilerplates` MCP tool from scaffold-mcp
- **Create new application**: Use `use-boilerplate` MCP tool from scaffold-mcp
- **List available features**: Use `list-scaffolding-methods` MCP tool from scaffold-mcp with `projectPath` parameter
- **Add new feature**: Use `use-scaffold-method` MCP tool from scaffold-mcp

### 2. Before Editing Files

**ALWAYS get design patterns and coding standards first:**

Use the `get_file_design_pattern` MCP tool from architect-mcp with the file path you're about to edit.

This returns:
- Project information and source template
- Applicable design patterns from architect.yaml
- Coding rules from RULES.yaml (must_do, should_do, mu
```

</details>
