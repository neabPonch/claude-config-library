---
name: kingkongshot__Pensieve
source: https://github.com/kingkongshot/Pensieve/blob/8731f61b18a65f09eb0d3cd1ffbff7650ef8df48/SKILL.md
repo: kingkongshot/Pensieve
kind: skill
stars: 2522
last_pushed: 2026-05-08T05:14:49Z
license: mit
score: 8
domains: [agents-ai, cli-tools, knowledge-management]
tags: [memory-management, self-improvement, architectural-decisions]
curated: 2026-06-14
curated_by: config-scout
---

# kingkongshot/Pensieve — skill

**Why it's worth keeping:** The 'self-improve' loop for extracting reusable conclusions and the graph-based state management are highly transferable techniques for long-term agent tasks.

**Summary:** Provides a sophisticated structured memory system that stores project decisions, module boundaries, and call chains in a local directory.

**Source credibility:** Very high; 2500+ stars and recent activity indicate it is a well-regarded community tool.

**Recency:** Current; designed as a sophisticated layer on top of modern agentic workflows.

**Source:** [kingkongshot/Pensieve/SKILL.md](https://github.com/kingkongshot/Pensieve/blob/8731f61b18a65f09eb0d3cd1ffbff7650ef8df48/SKILL.md) · 2522★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pensieve
description: >-
  Project knowledge base and workflow router. knowledge/ caches explored file
  locations, module boundaries, and call chains for reuse; decisions/maxims are
  established architecture decisions and coding standards to follow, not
  relitigate; pipelines are reusable workflows; short-term/ stages new
  conclusions until promotion or deletion. Use self-improve after completing
  work to capture new insights. Provides seven tools: init, upgrade, migrate,
  doctor, self-improve, refine, and sync-instructions.
---

# Pensieve

Route user requests to the correct tool. When in doubt, confirm first.

## Routing
- Init: Initialize the current project user-data directory and seed files. Tool spec: `.src/tools/init.md`.
- Upgrade: Refresh Pensieve skill source code in the global git clone. Tool spec: `.src/tools/upgrade.md`.
- Migrate: Run structural migration and legacy cleanup. Tool spec: `.src/tools/migrate.md`.
- Doctor: Read-only scan of the current project user-data directory. Tool spec: `.src/tools/doctor.md`.
- Self-Improve: Extract reusable conclusions and write them into user data. Tool spec: `.src/tools/self-improve.md`.
- Refine: Refine the know
```

</details>
