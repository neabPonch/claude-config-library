---
name: ritikakatta24-beep__autostack_ai
source: https://github.com/ritikakatta24-beep/autostack_ai/blob/4995087a1991cff565d9474744304463af561f56/claude.md
repo: ritikakatta24-beep/autostack_ai
kind: claude-md
stars: 0
last_pushed: 2026-04-11T08:56:31Z
license: unknown
score: 9
domains: [agents-ai, mobile-dev, fullstack, llm-orchestration]
tags: [multi-agent, flutter, firebase, workflow-automation]
curated: 2026-06-14
curated_by: config-scout
---

# ritikakatta24-beep/autostack_ai — claude-md

**Why it's worth keeping:** The mandatory 'Plan -> Validate Schema -> Code' pipeline prevents architectural drift; the detailed agent-to-file mapping and ML mode strategies are highly transferable for complex AI workflows.

**Summary:** Orchestrates a multi-agent workflow to transform descriptions into full-stack Flutter/Firebase apps using a single source of truth JSON schema.

**Source credibility:** Low (0 stars, unknown license), but shows high-level software architecture expertise.

**Recency:** Highly current; utilizes modern multi-agent orchestration patterns well-suited for Claude Code.

**Source:** [ritikakatta24-beep/autostack_ai/claude.md](https://github.com/ritikakatta24-beep/autostack_ai/blob/4995087a1991cff565d9474744304463af561f56/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AutoStack AI — Claude Instructions

## What This Project Is
AutoStack AI is a multi-agent system that converts a natural language app description into a complete, production-ready Flutter + Firebase application with optional ML integration.

## How to Start
When a user provides an app description, always run the **main workflow**:
```
.claude/workflows/main.md
```
Never skip the planner. Never write code before `system_plan.json` exists and is valid JSON.

---

## Agent Map

| Agent | File | Reads from system_plan.json | Purpose |
|---|---|---|---|
| Planner | `.claude/agents/planner.md` | — (writes the plan) | Converts prompt → `system_plan.json` |
| Builder | `.claude/agents/builder.md` | entire file | Coordinates the three builder sub-agents |
| Builder UI | `.claude/agents/builder/builder_ui.md` | `frontend.pages`, `backend.features`, `state_management` | Flutter scaffold + screens + state |
| Builder Firebase | `.claude/agents/builder/builder_firebase.md` | `backend.firebase_services`, `backend.features` | Auth + Firestore + Storage + Functions + rules |
| Builder DevOps | `.claude/agents/builder/builder_devops.md` | `deployment_target`, `backend.firebase_services` | CI/CD +
```

</details>
