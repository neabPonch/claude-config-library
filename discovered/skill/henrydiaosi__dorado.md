---
name: henrydiaosi__dorado
source: https://github.com/henrydiaosi/dorado/blob/9ac1a514a2c0eeea3c111133264bcd8662aa4f26/SKILL.md
repo: henrydiaosi/dorado
kind: skill
stars: 157
last_pushed: 2026-04-01T12:24:43Z
license: mit
score: 9
domains: [cli-tools, ai-agents, workflow-automation, software-engineering]
tags: [ospec, workflow, protocol, state-management]
curated: 2026-06-15
curated_by: config-scout
---

# henrydiaosi/dorado — skill

**Why it's worth keeping:** It utilizes specific file-existence checklists to prevent hallucinated completion and includes 'Anti-Drift Rules' that command the agent on exactly what not to do. This technique of defining a 'change-ready state' is highly effective for maintaining context in large projects.

**Summary:** A document-driven workflow that enforces a strict change-based lifecycle (Init -> Change -> Execute -> Archive) for AI-assisted development. It uses structured file paths as the ground truth for project state and knowledge maintenance.

**Source credibility:** Solid; 157 stars indicates community interest, and recent activity suggests it is actively maintained.

**Recency:** Very current; designed specifically as an operational layer for agentic CLI tools like Claude Code.

**Source:** [henrydiaosi/dorado/SKILL.md](https://github.com/henrydiaosi/dorado/blob/9ac1a514a2c0eeea3c111133264bcd8662aa4f26/SKILL.md) · 157★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ospec
description: Document-driven OSpec workflow for AI-assisted development with change-ready initialization, execution, validation, and archive readiness.
tags: [cli, workflow, automation, typescript, ospec, bootstrap]
---

# OSpec CLI

Document-driven OSpec workflow for AI-assisted development with change-ready initialization, execution, validation, archiving, and docs maintenance.

## Default Entry

When the user says something short like:

- `使用 ospec 初始化项目`
- `使用 ospec 初始化这个目录`
- `use ospec to initialize this directory`
- `use ospec to initialize this repo`

expand it internally as:

1. initialize the repository with `ospec init` so it ends in a change-ready state
2. if project context is missing and the AI can ask follow-up questions, ask one concise question for project summary or tech stack
3. if the user declines or the flow is CLI-only, continue with placeholder project docs
4. create the first change only when explicitly requested

Do not force the user to repeat those steps manually when the request is already clear.

Treat plain project-init intent as enough to trigger this flow. Do not require the user to restate the guardrails in a longer prompt.

## Mand
```

</details>
