---
name: Piyush-Goenka__Clawd
source: https://github.com/Piyush-Goenka/Clawd/blob/9bbb601674e4627c0810c0b12a406ea29c639237/Skill.md
repo: Piyush-Goenka/Clawd
kind: skill
stars: 0
last_pushed: 2026-04-25T23:01:17Z
license: mit
score: 8
domains: [cli-tools, agents-ai, typescript]
tags: [architecture-guide, tool-definition, system-patterns]
curated: 2026-06-14
curated_by: config-scout
---

# Piyush-Goenka/Clawd — skill

**Why it's worth keeping:** It provides concrete code templates for tool/command definitions and explains the system's permission logic—crucial for an agent to understand how to extend a complex codebase without breaking constraints.

**Summary:** A comprehensive architectural blueprint for a high-scale TypeScript CLI agent, detailing directory structures, startup sequences, and design patterns.

**Source credibility:** Low social proof (0 stars), but the technical density indicates a highly sophisticated, high-quality project structure.

**Recency:** Very recent; aligns with modern MCP and advanced tool-calling architectures.

**Source:** [Piyush-Goenka/Clawd/Skill.md](https://github.com/Piyush-Goenka/Clawd/blob/9bbb601674e4627c0810c0b12a406ea29c639237/Skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: clawd-skill
description: Development conventions and architecture guide for the Clawd CLI repository.
---

# Clawd — Repository Skill

## Project Overview

Clawd is a terminal coding assistant: file editing, shell commands, git workflows, code review, multi-agent coordination, IDE integration (VS Code, JetBrains), and Model Context Protocol (MCP), backed by the Anthropic API where configured.

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
| Analytics        | GrowthBook (feature flags & A/B testing)       |
| Pro
```

</details>
