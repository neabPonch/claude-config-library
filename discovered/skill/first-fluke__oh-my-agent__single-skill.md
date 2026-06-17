---
name: first-fluke__oh-my-agent__single-skill
source: https://github.com/first-fluke/oh-my-agent/blob/a44a119ae62a5e9337769057b136d0ea43e7641a/web/docs/guide/single-skill.md
repo: first-fluke/oh-my-agent
kind: skill
stars: 1085
last_pushed: 2026-06-14T13:42:09Z
license: mit
score: 9
domains: [agent-orchestration, prompt-engineering, software-engineering]
tags: [templates, workflows, structured-prompts]
curated: 2026-06-14
curated_by: config-scout
---

# first-fluke/oh-my-agent — skill

**Why it's worth keeping:** The 'Goal-Context-Constraints-Acceptance Criteria' template and the concept of a `CHARTER_CHECK` are elite patterns for reducing LLM ambiguity.

**Summary:** Provides a highly structured framework for single-domain agent tasks using standardized prompt templates and execution flows.

**Source credibility:** High; it comes from a highly-starred, actively maintained repository focused on agentic workflows.

**Recency:** Very current; perfectly aligns with modern agentic/coding assistant capabilities.

**Source:** [first-fluke/oh-my-agent/web/docs/guide/single-skill.md](https://github.com/first-fluke/oh-my-agent/blob/a44a119ae62a5e9337769057b136d0ea43e7641a/web/docs/guide/single-skill.md) · 1085★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
title: "Guide: Single Skill Execution"
description: Detailed guide for single-domain tasks in oh-my-agent, covering when to use, preflight checklist, prompt template with explanation, real examples for frontend, backend, mobile, and database tasks, expected execution flow, quality gate checklist, and escalation signals.
---

# Single Skill Execution

Single skill execution is the fast path: one agent, one domain, one focused task. No orchestration overhead, no multi-agent coordination. The skill auto-activates from your natural language prompt.

---

## When to use single skill

Use this when your task meets ALL of these criteria:

- **Owned by one domain**: the entire task belongs to frontend, backend, mobile, database, design, infrastructure, or another single domain
- **Self-contained**: no cross-domain API contract changes, no backend changes needed for a frontend task
- **Clear scope**: you know what the output should be (a component, an endpoint, a schema, a fix)
- **No coordination**: other agents do not need to run before or after

**Examples of single-skill tasks:**
- Build one UI component
- Add one API endpoint
- Fix one bug in one layer
- Design one database table
-
```

</details>
