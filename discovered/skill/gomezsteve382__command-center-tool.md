---
name: gomezsteve382__command-center-tool
source: https://github.com/gomezsteve382/command-center-tool/blob/b8fc0600f62c9aca156264a30b6865cad7733baf/Skill.md
repo: gomezsteve382/command-center-tool
kind: skill
stars: 0
last_pushed: 2026-05-22T04:18:56Z
license: mit
score: 8
domains: [cli-tools, agents-ai, architecture]
tags: [typescript, bun, ink-react, agentic-workflows]
curated: 2026-06-14
curated_by: config-scout
---

# gomezsteve382/command-center-tool — skill

**Why it's worth keeping:** The 'buildTool' factory pattern (integrating schema, permissions, and concurrency safety) is an excellent template for building robust agent tools. The distinction between PromptCommands and LocalCommands provides a sophisticated framework for LLM interaction design.

**Summary:** A comprehensive architectural blueprint for a high-performance agentic CLI built with TypeScript and Bun.

**Source credibility:** Low visibility/stars on GitHub, but the technical depth suggests high-level engineering expertise.

**Recency:** Extremely current, with activity within the last month.

**Source:** [gomezsteve382/command-center-tool/Skill.md](https://github.com/gomezsteve382/command-center-tool/blob/b8fc0600f62c9aca156264a30b6865cad7733baf/Skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: code-engine-skill
description: Development conventions and architecture guide for the Code Engine CLI repository.
---

# Code Engine — Repository Skill

## Project Overview

Code Engine is SRT Lab's CLI tool for interacting with Claude from the terminal. It supports file editing, shell commands, git workflows, code review, multi-agent coordination, IDE integration (VS Code, JetBrains), and Model Context Protocol (MCP).

**Codebase:** ~1,900 files, 512,000+ lines of TypeScript under `src/`.

## Tech Stack

| Component        | Technology                                      |
|------------------|------------------------------------------------|
| Language         | TypeScript (strict mode, ES modules)           |
| Runtime          | Bun (JSX support, `bun:bundle` feature flags)  |
| Terminal UI      | React + Ink (React for CLI)                    |
| CLI Parser       | Commander.js (`@commander-js/extra-typings`)   |
| API Client       | `@anthropic-ai/sdk`                            |
| Validation       | Zod v4                                         |
| Linter/Formatter | Biome                                          |
| Analytics        | GrowthBook (feature flags &
```

</details>
