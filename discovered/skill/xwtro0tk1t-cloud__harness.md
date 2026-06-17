---
name: xwtro0tk1t-cloud__harness
source: https://github.com/xwtro0tk1t-cloud/harness/blob/3e8bb50bc16aa8b706a2151e6b24a2966b2f8f19/SKILL.md
repo: xwtro0tk1t-cloud/harness
kind: skill
stars: 323
last_pushed: 2026-05-04T13:52:05Z
license: unknown
score: 8
domains: [ai-agents, cli-tools, devops]
tags: [scaffold, orchestration, meta-skill]
curated: 2026-06-14
curated_by: config-scout
---

# xwtro0tk1t-cloud/harness — skill

**Why it's worth keeping:** The pattern of detecting AI tools to select the correct rule file (e.g., CLAUDE.md vs .cursorrules) is highly transferable, as is the concept of an 'Agent Team' with specific roles/constraints to prevent context drift.

**Summary:** An orchestration meta-skill that automizes project 'Day 0' setup, including tool-specific instruction mapping, multi-agent role definitions, and documentation hierarchies.

**Source credibility:** Highly visible community project with significant stars and recent activity.

**Recency:** Extremely current; updated within the last month to reflect modern agentic workflows.

**Source:** [xwtro0tk1t-cloud/harness/SKILL.md](https://github.com/xwtro0tk1t-cloud/harness/blob/3e8bb50bc16aa8b706a2151e6b24a2966b2f8f19/SKILL.md) · 323★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Harness: Project Development Scaffold Meta-Skill

---
description: Use when the user wants to initialize a project development environment, establish a documentation system, set up an Agent Team, or says "harness", "project initialization", or "setup dev environment". Also automatically suggested at the first development session of a new project.
---

## Overview

Harness is a project development scaffold meta-skill. When invoked, it automatically: analyzes the project → installs/configures the shared Skill ecosystem → generates a documentation system → establishes an Agent Team → injects secure development standards.

**Core principles**:
1. **Assume beginner user** — Provide complete guidance, never skip steps
2. **Skills must be triggerable** — Not just installed, but hooks configured to ensure effectiveness
3. **Dual-layer enhancement + Skill auto-matching** — Hook (system-level) + CLAUDE.md (rule-level), Skill description assists automatic triggering
4. **Project-specific Skills stored separately** — Experience accumulated during development is saved to the project-level `.claude/skills/`
5. **Built-in security standards** — High-risk CWE defense + Agent behavior red lines
```

</details>
