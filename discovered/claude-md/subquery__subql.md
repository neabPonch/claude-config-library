---
name: subquery__subql
source: https://github.com/subquery/subql/blob/51e2a2c985c3c869510a36e8c37a3b3557af4a3c/CLAUDE.md
repo: subquery/subql
kind: claude-md
stars: 18792
last_pushed: 2026-04-01T02:17:48Z
license: gpl-3.0
score: 9
domains: [cli-tools, web3, monorepo]
tags: [typescript, agentic-workflow, monorepo-guide]
curated: 2026-06-15
curated_by: config-scout
---

# subquery/subql — claude-md

**Why it's worth keeping:** The specific pattern of writing detailed plans to `.claude/tasks/` to ensure handoff continuity and the mandate for human review before implementation are elite agentic techniques.

**Summary:** Establishes a rigorous planning-first workflow and provides deep architectural context for a complex TypeScript monorepo.

**Source credibility:** Highly credible; a major web3 project with 18k+ stars and recent activity.

**Recency:** Very current; mentions modern AI integrations like MCP.

**Source:** [subquery/subql/CLAUDE.md](https://github.com/subquery/subql/blob/51e2a2c985c3c869510a36e8c37a3b3557af4a3c/CLAUDE.md) · 18792★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.


## Plan and Reivew

### Before Starting work
- Always in planning mode, to make a plan
- After the plan is made, make sure to write the plan to ./.claude/tasks/TASK_NAME.md
- The plan should be a detailed implementation and the reasoning behind them as well as the tasks broken down
- If the task requires external knowledge or certain dependencies, also research to get the latest knowledge. (Use the Task tool for research)
- Don't over plan it, always design an MVP
- Once you make the plan, firstly ask me to review it . Do not continue until I approve the plan

### While implementing
- The plan should be updated as you work
- After completing tasks in the plan you should append a detailed description of the channges you made, so the following tasks can be handed over to other engineers

## Development Commands

### Building
- `yarn build` - Build all packages in the workspace using TypeScript
- Individual package builds use `tsc -b` and copy necessary files (e.g., CLI templates)

### Testing
- `yarn test` - Run Jest tests with coverage in UTC timezone
- `yarn test:ci
```

</details>
