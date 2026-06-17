---
name: ai-shifu__ai-shifu
source: https://github.com/ai-shifu/ai-shifu/blob/c3fea45dd6da17074076bc749974315d438f0b38/SKILL.md
repo: ai-shifu/ai-shifu
kind: skill
stars: 295
last_pushed: 2026-06-14T11:21:01Z
license: apache-2.0
score: 7
domains: [architectural-patterns, ai-agent-ops, developer-experience]
tags: [hierarchy, scalability, knowledge-management]
curated: 2026-06-14
curated_by: config-scout
---

# ai-shifu/ai-shifu — skill

**Why it's worth keeping:** Prevents monolithic configuration bloat by enforcing knowledge locality, ensuring the agent accesses task-specific context without saturating the global prompt.

**Summary:** Establishes a decentralized documentation hierarchy that distributes skill-specific instructions and troubleshooting workflows into local subproject files.

**Source credibility:** Active project with recent updates and moderate community recognition.

**Recency:** Highly relevant for managing scale-related context limitations in modern AI coding workflows.

**Source:** [ai-shifu/ai-shifu/SKILL.md](https://github.com/ai-shifu/ai-shifu/blob/c3fea45dd6da17074076bc749974315d438f0b38/SKILL.md) · 295★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ai-shifu Skills Entry

## Scope

- This file only keeps repository-level skill routing and boundary notes.
- Backend and frontend maintain their own skill entry points so this file does not grow into a mixed troubleshooting manual.

## Placement Rules

- Keep `ai-shifu/SKILL.md` for cross-project skill routing, ownership boundaries, and migration notes.
- Keep `src/api/SKILL.md` for backend project-level skill entry points and focused skill indexes.
- Keep `src/cook-web/SKILL.md` for long-lived cook-web constraints and focused skill indexes.
- Keep `src/api/skills/xxx/SKILL.md` or `src/cook-web/skills/xxx/SKILL.md` for focused skills with triggers, workflows, and regression checklists.

## Entry Points

- Backend: `src/api/SKILL.md`
- Frontend: `src/cook-web/SKILL.md`
- Frontend skills index: `src/cook-web/skills/README.md`
- Backend skills index: `src/api/skills/README.md`

## Migration Notes

- Stable rules belong in layered `AGENTS.md / CLAUDE.md`.
- Troubleshooting knowledge that needs step-by-step execution or long-term reuse belongs in the relevant subproject `SKILL.md` system.
```

</details>
