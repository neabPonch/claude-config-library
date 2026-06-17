---
name: s-andthat__palantir-ai-fde-library
source: https://github.com/s-andthat/palantir-ai-fde-library/blob/014486a9f3409766139e372c9d027ac9f2d61b97/skill.md
repo: s-andthat/palantir-ai-fde-library
kind: skill
stars: 5
last_pushed: 2026-03-16T00:32:19Z
license: mit
score: 9
domains: [agents-ai, data-engineering, enterprise-workflows]
tags: [skill-registry, capability-schema, safety-first]
curated: 2026-06-14
curated_by: config-scout
---

# s-andthat/palantir-ai-fde-library — skill

**Why it's worth keeping:** The schema requires 'Minimum Context' and 'Infrastructure Risk', which prevents agents from acting on insufficient or dangerous data. This provides a perfect template for defining tool-calling boundaries in complex environments.

**Summary:** A structured capability registry that defines atomic agent skills with rigorous safety and context parameters.

**Source credibility:** High; highly specific to Palantir FDE workflows with recent maintenance (3 months ago).

**Recency:** Current; the structured approach to capability management is highly relevant to modern agentic orchestration.

**Source:** [s-andthat/palantir-ai-fde-library/skill.md](https://github.com/s-andthat/palantir-ai-fde-library/blob/014486a9f3409766139e372c9d027ac9f2d61b97/skill.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# skill.md — AI FDE Atomic Capability Registry

> This file catalogs every discrete, reusable skill an AI FDE session can perform, independent of Mode.
> Each skill is an atomic unit — the smallest meaningful action the agent can take.
> Skills are composed into agents (see `agents.md`) and referenced in prompt files.

---

## Schema

| Field | Description |
|-------|-------------|
| **Skill ID** | Short slug used in agents.md and prompt files |
| **Skill Name** | Human-readable label |
| **Compatible Modes** | Which official Palantir Modes this skill applies to |
| **Required Tools** | Foundry tools that must be enabled in the session |
| **Minimum Context** | What the agent must be given to perform this skill |
| **Branch Required** | Whether a branch proposal is mandatory |
| **Infrastructure Risk** | Low / Medium / High |
| **Notes** | Known behaviors, caveats, or tips |

---

## Transform Skills

### `transform.create-python`
**Skill Name:** Create Python Transform  
**Compatible Modes:** Data Integration  
**Required Tools:** Code Repository, Transform Preview  
**Minimum Context:** Source dataset path, target object type or dataset name, transform logic description  
**Branc
```

</details>
