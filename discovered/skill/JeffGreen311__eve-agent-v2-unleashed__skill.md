---
name: JeffGreen311__eve-agent-v2-unleashed__skill
source: https://github.com/JeffGreen311/eve-agent-v2-unleashed/blob/06a63495de73615ba77eccb177e7772e4e8f3055/.claude/skills/cc-tool-descriptions/SKILL.md
repo: JeffGreen311/eve-agent-v2-unleashed
kind: skill
stars: 36
last_pushed: 2026-06-01T21:21:36Z
license: mit
score: 8
domains: [ai-agents, cli-tools, automation]
tags: [tool-reference, agentic-workflows, background-monitoring]
curated: 2026-06-15
curated_by: config-scout
---

# JeffGreen311/eve-agent-v2-unleashed — skill

**Why it's worth keeping:** It provides highly actionable shell/node patterns for creating event streams (the 'Background monitor' section) which is critical for building sophisticated autonomous workflows.

**Summary:** A high-density technical reference defining the advanced capabilities of Claude Code's toolset, specifically regarding agent orchestration and background monitoring.

**Source credibility:** Moderate; 36 stars suggests a niche but growing interest in local-first agentic tools.

**Recency:** Current; reflects advanced Claude Code features like worktree isolation and the HTML 'preview' field.

**Source:** [JeffGreen311/eve-agent-v2-unleashed/.claude/skills/cc-tool-descriptions/SKILL.md](https://github.com/JeffGreen311/eve-agent-v2-unleashed/blob/06a63495de73615ba77eccb177e7772e4e8f3055/.claude/skills/cc-tool-descriptions/SKILL.md) · 36★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Tool Descriptions Reference


---

## Tool Description: Agent (simple usage notes)

${TOOL_BASE_DESCRIPTION}${HAS_PRO_RESTRICTION_NOTE?"":`

## When to use

Reach for this when the task matches an available agent type, when you have independent work to run in parallel, or when answering would mean reading across several files — delegate it and you keep the conclusion, not the file dumps. For a single-fact lookup where you already know the file, symbol, or value, search directly. Once you've delegated a search, don't also run it yourself — wait for the result.`}${CAN_FORK_CONTEXT?`

A fork runs in the background and keeps its tool output out of your context. If you are the fork, execute directly — don't re-delegate.`:""}

- The agent's final message is returned to you as the tool result; it is not shown to the user — relay what matters.
- Use ${SEND_MESSAGE_TOOL_NAME} with the agent's ID or name to continue a previously spawned agent with its context intact; a new ${AGENT_TOOL_NAME} call${CAN_FORK_CONTEXT?" with a subagent_type":""} starts fresh.
- `isolation: "worktree"` gives the agent its own git worktree (auto-cleaned if unchanged).${RUN_IN_BACKGROUND_NOTE}${PARALL
```

</details>
