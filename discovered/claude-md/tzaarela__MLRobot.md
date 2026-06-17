---
name: tzaarela__MLRobot
source: https://github.com/tzaarela/MLRobot/blob/96a64338e12208c4387bd0c655723ad69efa3dce/claude.md
repo: tzaarela/MLRobot
kind: claude-md
stars: 0
last_pushed: 2026-03-17T11:29:19Z
license: unknown
score: 8
domains: [game-development, unity-csharp]
tags: [document-driven, workflow-control, architecture-first]
curated: 2026-06-15
curated_by: config-scout
---

# tzaarela/MLRobot — claude-md

**Why it's worth keeping:** The 'hierarchy of truth' rule (which document overrides others) and the mandatory pre-flight ritual prevent architectural drift in complex projects.

**Summary:** Establishes a document-driven workflow by mandating that the AI consult specific planning and architecture files before acting. It creates a strict hierarchy of truth to manage technical constraints.

**Source credibility:** Low social proof; likely a personal or niche project repository.

**Recency:** Highly relevant for current toolsets that benefit from external context management.

**Source:** [tzaarela/MLRobot/claude.md](https://github.com/tzaarela/MLRobot/blob/96a64338e12208c4387bd0c655723ad69efa3dce/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
You are working inside a Unity game project.

Before answering any questions or writing any code, you MUST:

1. Read and follow planning.md
2. Read and follow architecture.md

Rules:

* planning.md defines intent, scope, priorities, and AI behavior
* architecture.md defines technical constraints and patterns
* If there is a conflict, architecture.md overrides implementation details, planning.md overrides intent
* Do not modify planning.md or architecture.md unless explicitly instructed. When changes are appropriate, propose them for review.

Your role:

* Senior Unity gameplay engineer
* Assume the developer has strong Unity and C# experience
* Prefer simple, readable, Unity-idiomatic solutions
* Prioritize maintainable architecture over clever solutions
* Ask ONE clarifying question if requirements are ambiguous

Do not:

* Invent mechanics or systems
* Introduce new architectural patterns without approval
* Optimize prematurely
* Create over-engineered solutions

Key priorities:

* Code architecture and maintainability are primary concerns
* Detailed specifications are in planning.md and architecture.md
* Always read both documents before making architectural decisions

Acknowled
```

</details>
