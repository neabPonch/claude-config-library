---
name: mintuz__claude-plugins
source: https://github.com/mintuz/claude-plugins/blob/280c015271cbf539f7950469df6f515cc41be6ec/CLAUDE.md
repo: mintuz/claude-plugins
kind: claude-md
stars: 20
last_pushed: 2026-01-29T20:16:03Z
license: mit
score: 8
domains: [agents-ai, cli-tools, developer-experience]
tags: [plugin-system, agent-framework, structured-prompts]
curated: 2026-06-15
curated_by: config-scout
---

# mintuz/claude-plugins — claude-md

**Why it's worth keeping:** The 'WHEN/NOT' naming convention for agent descriptions is a brilliant way to prevent tool misapplication, and the YAML-based specification format provides excellent structure for complex workflows.

**Summary:** Establishes a highly structured plugin architecture that categorizes AI capabilities into Agents (active), Skills (contextual knowledge), and Commands (quick actions).

**Source credibility:** Niche repository with high-quality documentation density despite modest star count.

**Recency:** Current; reflects modern patterns of MCP and autonomous agent orchestration.

**Source:** [mintuz/claude-plugins/CLAUDE.md](https://github.com/mintuz/claude-plugins/blob/280c015271cbf539f7950469df6f515cc41be6ec/CLAUDE.md) · 20★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Claude Code plugin marketplace containing seven plugins for software development and personal productivity workflows:

- **core** – memory, commit hygiene, refactoring, prompt refinement, and branch review
- **web** – CSS, React, Tailwind, testing, refactoring, and design practices
- **typescript** – strict, schema-first TypeScript guidance
- **system-design** – Mermaid diagram generation from code
- **product-management** – PRD creation, status updates, and task orchestration
- **app** – Swift iOS testing, App Intent-first development, and SwiftUI architecture
- **life** – personal life management with GPS method for goal achievement

## Plugin Architecture

Plugins extend Claude Code with three types of content:

1. **Agents** - Autonomous subprocesses with specialized tools and context (defined in `agents/*.md`)
2. **Skills** - Knowledge bases that load into context (defined in `skills/*/SKILL.md`)
3. **Commands** - Slash commands for quick actions (defined in `commands/*.md`)

The marketplace registry (`.claude-plugin/marketplace.json`) index
```

</details>
