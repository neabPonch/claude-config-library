---
name: enulus__OpenPackage__agents-claude
source: https://github.com/enulus/OpenPackage/blob/399187d6cc4f4c86391fa07ff23b5387f898d2bf/specs/agents-claude.md
repo: enulus/OpenPackage
kind: claude-md
stars: 577
last_pushed: 2026-05-29T11:02:53Z
license: apache-2.0
score: 9
domains: [agents-ai, cli-tools]
tags: [subagents, agentic-workflows]
curated: 2026-06-15
curated_by: config-scout
---

# enulus/OpenPackage — claude-md

**Why it's worth keeping:** It provides a clear schema for isolating task-specific context and tool permissions through structured metadata (tools, model, permissionMode).

**Summary:** Defines a rigorous framework for creating specialized AI subagents using Markdown files with YAML frontmatter.

**Source credibility:** High-quality open-source project with 577 stars and active maintenance.

**Recency:** Highly current; last updated within the past month.

**Source:** [enulus/OpenPackage/specs/agents-claude.md](https://github.com/enulus/OpenPackage/blob/399187d6cc4f4c86391fa07ff23b5387f898d2bf/specs/agents-claude.md) · 577★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Subagents

> Create and use specialized AI subagents in Claude Code for task-specific workflows and improved context management.

Custom subagents in Claude Code are specialized AI assistants that can be invoked to handle specific types of tasks. They enable more efficient problem-solving by providing task-specific configurations with customized system prompts, tools and a separate context window.

## What are subagents?

Subagents are pre-configured AI personalities that Claude Code can delegate tasks to. Each subagent:

* Has a specific purpose and expertise area
* Uses its own context window separate from the main conversation
* Can be configured with specific tools it's allowed to use
* Includes a custom system prompt that guides its behavior

When Claude Code encounters a task that matches a subagent's expertise, it can delegate that task to the specialized subagent, which works independently and returns results.

## Key benefits

<CardGroup cols={2}>
  <Card title="Context preservation" icon="layer-group">
    Each subagent operates in its own context, preventing pollution of the main conversation and keeping it focused on high-level objectives.
  </Card>

  <Card title="Sp
```

</details>
