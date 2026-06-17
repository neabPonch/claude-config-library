---
name: baekenough__oh-my-customcode__claude-en
source: https://github.com/baekenough/oh-my-customcode/blob/fe6c91fefd1bc5277914b5ecf359bcda4e0b3ff3/templates/CLAUDE.md.en
repo: baekenough/oh-my-customcode
kind: claude-md
stars: 27
last_pushed: 2026-06-14T01:15:01Z
license: mit
score: 9
domains: [agents-ai, cli-tools, devops]
tags: [agentic-framework, multi-agent, orchestration, structured-workflows]
curated: 2026-06-15
curated_by: config-scout
---

# baekenough/oh-my-customcode — claude-md

**Why it's worth keeping:** Demonstrates high-level 'enforcement' techniques where the model must self-correct its identity/format; shows how to structure complex toolsets via specialized agent sub-directories.

**Summary:** An advanced agentic orchestration framework that transforms Claude Code into a highly structured multi-agent system. It uses strict enforcement rules to ensure consistent agent identification, tool usage, and task decomposition.

**Source credibility:** High-effort repository with recent activity and a sophisticated, non-generic architectural design.

**Recency:** Very current; integrates advanced Claude Code features like experimental Agent Teams.

**Source:** [baekenough/oh-my-customcode/templates/CLAUDE.md.en](https://github.com/baekenough/oh-my-customcode/blob/fe6c91fefd1bc5277914b5ecf359bcda4e0b3ff3/templates/CLAUDE.md.en) · 27★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AI Agent System

Powered by oh-my-customcode.

---
## STOP AND READ BEFORE EVERY RESPONSE

1. Response starts with agent identification? (R007) 2. Tool calls include identification? (R008) 3. Spawning 2+ agents? Check R018. → If NO to any, FIX IMMEDIATELY

---

## CRITICAL: Scope of Rules

> **These rules apply ALWAYS, regardless of context:**

| Context | Rules Apply? |
|---------|-------------|
| Working on this project | **YES** |
| Working on external projects | **YES** |
| After context compaction | **YES** |
| Simple questions | **YES** |
| ANY situation | **YES** |

---

## CRITICAL: Session Continuity

> **These rules apply at ALL times, including after context compaction.**

```
When a session continues after "compact conversation":
1. RE-READ this CLAUDE.md IMMEDIATELY
2. ALL enforcement rules remain ACTIVE
3. Previous context summary does NOT override these rules
4. First response MUST include agent identification

NO EXCEPTIONS. NO EXCUSES.
```

---

## CRITICAL: Enforcement Rules

> **These rules are NON-NEGOTIABLE. Violation = immediate correction required.**

| Rule | Core | On Violation |
|------|------|-------------|
| R007 Agent ID | Every response starts with `
```

</details>
