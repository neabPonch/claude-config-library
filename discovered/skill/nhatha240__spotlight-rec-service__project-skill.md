---
name: nhatha240__spotlight-rec-service__project-skill
source: https://github.com/nhatha240/spotlight-rec-service/blob/e443c11c8fdf07c91de6577fa06fda014a538ea8/PROJECT_SKILL.md
repo: nhatha240/spotlight-rec-service
kind: skill
stars: 0
last_pushed: 2026-04-01T09:09:05Z
license: unknown
score: 7
domains: [architecture, ai-orchestration]
tags: [router, skill-dispatcher, policy-driven]
curated: 2026-06-15
curated_by: config-scout
---

# nhatha240/spotlight-rec-service — skill

**Why it's worth keeping:** The 'Invocation Policy' provides a clear hierarchy for crossing technical layers, and the mandated return types (SignalResult) enforce consistent reasoning protocols across different languages.

**Summary:** A centralized skill dispatcher that routes the agent to specialized domain documents based on task complexity and technical boundaries.

**Source credibility:** Low; 0 stars indicates this is likely a private or emerging project structure.

**Recency:** 

**Source:** [nhatha240/spotlight-rec-service/PROJECT_SKILL.md](https://github.com/nhatha240/spotlight-rec-service/blob/e443c11c8fdf07c91de6577fa06fda014a538ea8/PROJECT_SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project Skill Router

This file is the skill dispatcher for the repository.

## Skill Catalog (Call Only When Needed)
- `docs/skills/frontend-skill.md`: UI architecture, component composition, accessibility, frontend performance.
- `docs/skills/backend-skill.md`: service boundaries, API/domain flow, persistence and queue integration.
- `docs/skills/python-skill.md`: Python implementation, validation, API handlers, data and ML pipeline jobs.
- `docs/skills/rust-skill.md`: high-throughput pipelines, low-latency processors, memory-safe hot paths.
- `docs/skills/gateway-skill.md`: API Gateway, auth, routing policy, rate limiting, request shaping.
- `docs/skills/devops-skill.md`: deployment, CI/CD, observability, incident response, SLO operations.

## Invocation Policy
1. Default to no skill.
2. Call exactly one primary skill for focused tasks.
3. Call extra skill(s) only when the task crosses clear technical boundaries.
4. For mixed tasks, apply skills in this order:
   - `gateway` -> `backend` -> `python` or `rust` -> `devops` -> `frontend`

## Non-Negotiable Rules
- Keep code and docs production-ready and testable.
- Never hardcode environment or infrastructure values.
- Every deci
```

</details>
