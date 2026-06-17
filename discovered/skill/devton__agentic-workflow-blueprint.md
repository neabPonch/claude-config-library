---
name: devton__agentic-workflow-blueprint
source: https://github.com/devton/agentic-workflow-blueprint/blob/7e97ee82ec647751340a1202989f446723fa9d11/SKILL.md
repo: devton/agentic-workflow-blueprint
kind: skill
stars: 57
last_pushed: 2026-05-24T21:54:13Z
license: unknown
score: 9
domains: [agent-orchestration, devops-automation, documentation-systems]
tags: [blueprint, workflow-engine, meta-instruction]
curated: 2026-06-15
curated_by: config-scout
---

# devton/agentic-workflow-blueprint — skill

**Why it's worth keeping:** The 'Executable Contract' structure (Goal/Scope/Invariants/Procedure) is a top-tier way to ensure deterministic agent behavior; the command routing pattern allows for complex orchestration without overwhelming the root documentation.

**Summary:** A meta-blueprint for scaffolding an agentic command hierarchy that organizes project logic into modular 'skills' and 'workflows'. It uses a routing pattern to prevent context bloat via progressive disclosure.

**Source credibility:** Moderately high-quality logic despite relatively low star count, demonstrating sophisticated understanding of LLM instruction patterns.

**Recency:** Very current; aligns perfectly with advanced Claude Code/MCP workflow requirements.

**Source:** [devton/agentic-workflow-blueprint/SKILL.md](https://github.com/devton/agentic-workflow-blueprint/blob/7e97ee82ec647751340a1202989f446723fa9d11/SKILL.md) · 57★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: workflow-blueprint
description: Blueprint workflow to scaffold agent-oriented documentation with progressive disclosure and executable contracts.
---

## agentic-workflows.blueprint

### Goal

Provide a reusable blueprint workflow that scaffolds an "agentic workflows" documentation structure for any codebase, with progressive disclosure and executable contracts (workflows).

### Scope

- Applies to: any repository that wants an agent-oriented documentation system (orchestrator + workflow skills + references + runbooks).
- Does not cover: implementing product features; this is scaffolding/documentation only.

### Triggers

- "Create agentic workflow structure"
- "Set up skills folder + workflows"
- "Make docs agent-friendly"
- "Refactor AGENTS.md into linked skills"

### Inputs

- `projectSlug`: short identifier for the repo (e.g. `my-backend`)
- `baseBranch`: default integration branch (e.g. `develop`, `main`)
- `techStack`: short list (e.g. `NestJS + MikroORM + Graphile Worker`)
- `existingRootDoc`: root instruction file path (`AGENTS.md`, `CLAUDE.md`, etc.)
- `workflowsWanted`: list of workflow ids to scaffold (e.g. `modules`, `specs`, `document`, `plan-to-blueprint`)
-
```

</details>
