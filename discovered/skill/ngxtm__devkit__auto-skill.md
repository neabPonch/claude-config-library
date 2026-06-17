---
name: ngxtm__devkit__auto-skill
source: https://github.com/ngxtm/devkit/blob/9439f27ce3fa7fe53ff9278a1ee9a44bffa70eba/rules/base/auto-skill.md
repo: ngxtm/devkit
kind: skill
stars: 7
last_pushed: 2026-02-28T04:39:21Z
license: mit
score: 8
domains: [cli-tools, agents-ai, workflow-automation]
tags: [discovery-engine, context-management, meta-skill]
curated: 2026-06-15
curated_by: config-scout
---

# ngxtm/devkit — skill

**Why it's worth keeping:** The 'manifest-first' approach (using skills-compact.json) allows an agent to navigate massive domain knowledge without bloating the context window until specific expertise is required.

**Summary:** A meta-skill orchestration system that uses a compact manifest to detect, suggest, and load specialized expertise on demand.

**Source credibility:** Low star count but demonstrates a highly sophisticated architectural pattern for multi-agent skill management.

**Recency:** Very current; aligns perfectly with modern agentic workflows and local-first tool use.

**Source:** [ngxtm/devkit/rules/base/auto-skill.md](https://github.com/ngxtm/devkit/blob/9439f27ce3fa7fe53ff9278a1ee9a44bffa70eba/rules/base/auto-skill.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Auto-Skill Detection

> Automatically detect and suggest relevant skills based on user's task

## When to Activate

Before starting ANY coding task, check if a relevant skill exists:

1. **Analyze** the user's request — extract key technologies, patterns, or domains
2. **Search** `skills-compact.json` for matching skill names/descriptions
3. **Suggest** top 1-3 matching skills with name and category
4. **Load** on user confirmation — read full skill from `skills/{name}/SKILL.md`

## Skill Categories

| Code | Category | Examples |
|------|----------|----------|
| `fe` | Frontend | react, vue, nextjs, tailwind, ui/ux |
| `be` | Backend | node, express, nestjs, fastapi, api |
| `db` | Database | postgres, mysql, mongodb, redis, prisma |
| `ai` | AI/ML | llm, agents, rag, mcp, embeddings |
| `ops` | DevOps | docker, k8s, ci/cd, aws, terraform |
| `test` | Testing | jest, playwright, tdd, e2e |
| `sec` | Security | auth, oauth, jwt, owasp, pentest |
| `git` | Git/Workflow | pr, review, commit, branching |
| `mob` | Mobile | react-native, flutter, ios, android |
| `py` | Python | django, flask, fastapi, pandas |
| `go` | Golang | gin, echo, fiber, concurrency |

## How to Search

1. R
```

</details>
