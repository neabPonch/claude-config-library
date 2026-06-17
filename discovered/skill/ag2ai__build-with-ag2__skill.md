---
name: ag2ai__build-with-ag2__skill
source: https://github.com/ag2ai/build-with-ag2/blob/29eeac374d18003696d8725d88e76d20176034a1/.agents/skills/ag2-hitl/SKILL.md
repo: ag2ai/build-with-ag2
kind: skill
stars: 245
last_pushed: 2026-06-16T02:51:54Z
license: apache-2.0
score: 8
domains: [agents-ai, security, cli-tools]
tags: [hitl, middleware, tool-calling, safety]
curated: 2026-06-16
curated_by: config-scout
---

# ag2ai/build-with-ag2 — skill

**Why it's worth keeping:** Provides a critical distinction between qualitative interaction (asking questions) and quantitative safety gates (approving actions), while documenting production risks like event-loop blocking and missing timeouts.

**Summary:** Outlines two essential human-in-the-loop patterns: gathering mid-execution input via a context hook and gating sensitive tool calls through approval middleware.

**Source credibility:** High; derived from the official AG2 (formerly AutoGen) sample repository.

**Recency:** Current; utilizes modern async/await patterns essential for today's agentic frameworks.

**Source:** [ag2ai/build-with-ag2/.agents/skills/ag2-hitl/SKILL.md](https://github.com/ag2ai/build-with-ag2/blob/29eeac374d18003696d8725d88e76d20176034a1/.agents/skills/ag2-hitl/SKILL.md) · 245★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ag2-hitl
description: Pause an AG2 beta `Agent` mid-run to collect human input via `context.input()`, or gate a tool call with `approval_required()` middleware. Use when the user wants the agent to ask for confirmation, request missing info (passwords, API keys, data), or have a human approve sensitive / irreversible / expensive tool calls (sending emails, deleting records, payments).
license: Apache-2.0
---

# Human-in-the-loop

## When to use

- The agent should **ask for confirmation** before doing something risky.
- The agent needs **information from the user mid-conversation** (a password, an API key, missing context).
- A specific **tool call should require human approval** before it runs (irreversible / expensive / sensitive).
- Quality assurance — show a draft, get human edits/approval before finalising.

Two distinct mechanisms — pick by intent:

| Need | Use |
|---|---|
| Tool asks an open question and waits for a typed answer | `context.input()` from inside the tool + `hitl_hook` on the agent |
| Approve / deny a specific tool call before its body runs | `approval_required()` tool middleware |

## Pattern 1 — `context.input()` for open questions

A tool request
```

</details>
