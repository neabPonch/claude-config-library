---
name: langroid__langroid__skill
source: https://github.com/langroid/langroid/blob/deb79824cb34f129b42c593fa7232f0e84b5a547/plugins/langroid/skills/patterns/SKILL.md
repo: langroid/langroid
kind: skill
stars: 4040
last_pushed: 2026-06-14T21:19:00Z
license: mit
score: 8
domains: [agents-ai, llm-orchestration]
tags: [design-patterns, tool-calling, stateful-agents]
curated: 2026-06-14
curated_by: config-scout
---

# langroid/langroid — skill

**Why it's worth keeping:** It outlines critical production techniques such as tool output validation against internal agent state and precise task termination via specific tool sequences.

**Summary:** A high-level index of architectural design patterns for building robust, stateful multi-agent systems.

**Source credibility:** High; Langroid is a highly-starred (4k+) and actively maintained framework for multi-agent programming.

**Recency:** Current; specifically includes modern Model Context Protocol (MCP) integration patterns.

**Source:** [langroid/langroid/plugins/langroid/skills/patterns/SKILL.md](https://github.com/langroid/langroid/blob/deb79824cb34f129b42c593fa7232f0e84b5a547/plugins/langroid/skills/patterns/SKILL.md) · 4040★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: patterns
description: Design patterns for the Langroid multi-agent LLM framework. Covers
  agent configuration, tools, task control, and integrations.
---

# Langroid Patterns

## Instructions

Below is an INDEX of design patterns organized by category. Each item describes
WHAT you might want to implement, followed by a REFERENCE to a document with
a complete code example.

Scan this index to find patterns matching your needs, then consult the
corresponding document.

---

## Agent & Task Basics

1. **Task Returns Tool Directly**

   Create a Langroid Agent equipped with a single Tool (a ToolMessage), and wrap
   it in a Task so that running the task returns that ToolMessage directly. Use
   this pattern when you want a simple LLM agent that returns a structured
   response.

   - Reference: `./task-return-tool.md`

---

## Tool Handlers

2. **Stateful Handler on Agent**

   Define a STATEFUL tool handler as a METHOD on the agent (not inside the
   ToolMessage). Use this pattern when: (a) the tool handler needs to execute
   external operations (API calls, database queries, file I/O), (b) you need to
   track state across retries (e.g., failure counter), (c) the handler n
```

</details>
