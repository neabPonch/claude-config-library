---
name: lmorchard__decafclaw__project-skill
source: https://github.com/lmorchard/decafclaw/blob/f80911aca84e83ae65bb46daeb9d3bbe5772d12c/docs/project-skill.md
repo: lmorchard/decafclaw
kind: skill
stars: 9
last_pushed: 2026-06-13T00:10:22Z
license: unknown
score: 8
domains: [agents-ai, workflow-automation, cli-tools]
tags: [state-machine, structured-workflows, persistence]
curated: 2026-06-15
curated_by: config-scout
---

# lmorchard/decafclaw — skill

**Why it's worth keeping:** The explicit lifecycle (brainstorm → spec → plan → execute) with formal backward transitions allows the agent to handle unexpected discoveries through structured replanning.

**Summary:** Implements a structured state machine for complex tasks using persistent markdown artifacts as a source of truth.

**Source credibility:** Low star count, but demonstrates high-level architectural thinking typical of advanced agentic system design.

**Recency:** Current; utilizes modern patterns for managing long-running agent workflows and context persistence.

**Source:** [lmorchard/decafclaw/docs/project-skill.md](https://github.com/lmorchard/decafclaw/blob/f80911aca84e83ae65bb46daeb9d3bbe5772d12c/docs/project-skill.md) · 9★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project Skill

Structured workflow for complex multi-step tasks. Guides the agent through
a lifecycle of brainstorm → spec → plan → execute → done, with persistent
markdown artifacts at each stage.

## When to use

Any task involving 3+ steps, research, or work spanning multiple turns.
Not for quick one-off questions.

## State machine

```
brainstorming → spec_review → planning → plan_review → executing → done
```

Backward transitions are supported:
- `spec_review → brainstorming` (refine spec)
- `plan_review → planning` (refine plan)
- `executing → planning` (replan based on discoveries)
- `executing → brainstorming` (fundamental rethink)

## Project directory

```
workspace/projects/{YYYY-MM-DD-HHMM}-{slug}/
  project.json    # State metadata
  spec.md         # Specification
  plan.md         # Structured plan with step checklist
  notes.md        # Timestamped notes
  {other files}   # Research, scratch, intermediate outputs
```

## Plan format

Steps use a markdown checklist with status markers:

```markdown
- [ ] 1. Pending step
- [>] 2. In-progress step
- [x] 3. Done step
  > Completed: What was accomplished.
- [-] 4. Skipped step
  > Skipped: Why it was skipped.
```

Su
```

</details>
