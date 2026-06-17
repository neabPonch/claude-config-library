---
name: goat-io__fluent__talk-to-claude
source: https://github.com/goat-io/fluent/blob/1a488c02a18e05f32a8d69a6b13e497f85bef6d9/.claude/commands/talk-to-claude.md
repo: goat-io/fluent
kind: claude-md
stars: 7
last_pushed: 2026-06-13T03:37:01Z
license: mit
score: 7
domains: [agents-ai, cli-tools, software-architecture]
tags: [subagents, parallel-processing, task-tool]
curated: 2026-06-15
curated_by: config-scout
---

# goat-io/fluent — claude-md

**Why it's worth keeping:** Provides highly structured YAML templates for delegation and demonstrates how to categorize subagents by domain-specific roles.

**Summary:** Defines a framework for spawning parallel Claude instances via the Task tool to perform specialized domain analysis.

**Source credibility:** Niche repository with high technical depth in agentic workflows.

**Recency:** Current; focuses on advanced task-based orchestration patterns.

**Source:** [goat-io/fluent/.claude/commands/talk-to-claude.md](https://github.com/goat-io/fluent/blob/1a488c02a18e05f32a8d69a6b13e497f85bef6d9/.claude/commands/talk-to-claude.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: claude-subagent
description: |
  Get a second opinion or parallel analysis from another Claude instance. Use this skill when:
  - User asks to "talk to Claude", "ask another Claude", or "get a second opinion"
  - User wants collaborative analysis or brainstorming
  - User wants to compare different approaches to a problem
  Requires: Task tool with general-purpose subagent.
---

# Claude Subagent Interaction

Spawn a separate Claude instance for parallel analysis or second opinions.

## Why Use This?

Unlike Gemini or ChatGPT (which require browser automation), Claude can spawn subagents directly using the Task tool. This is:
- **Faster** - No browser overhead
- **More reliable** - No DOM selectors to break
- **Context-aware** - Subagent can access the codebase

## How to Use

### Simple Second Opinion

```yaml
Tool: Task
Parameters:
  subagent_type: "general-purpose"
  prompt: |
    I need a second opinion on the following:

    [TOPIC OR QUESTION HERE]

    Please provide your independent analysis without being influenced by any prior context.
```

### Code Review

```yaml
Tool: Task
Parameters:
  subagent_type: "general-purpose"
  prompt: |
    Please review the follow
```

</details>
