---
name: saidmss-ux__said-repository-5-automation-workflow
source: https://github.com/saidmss-ux/said-repository-5-automation-workflow/blob/22d9980963c380e77263b38d2c1130181070225a/skill.md
repo: saidmss-ux/said-repository-5-automation-workflow
kind: skill
stars: 0
last_pushed: 2026-02-27T11:53:07Z
license: gpl-3.0
score: 7
domains: [python, automation, data-engineering]
tags: [contract-driven, validation-logic, pipeline-orchestration]
curated: 2026-06-14
curated_by: config-scout
---

# saidmss-ux/said-repository-5-automation-workflow — skill

**Why it's worth keeping:** Uses 'Data Contract Rules' and a structured 'Validation Mode' to force the agent to verify its own work against a source of truth rather than assuming success.

**Summary:** A strict engineering contract defining modularity and schema enforcement for a Python automation pipeline.

**Source credibility:** Low; the repository has zero stars and limited social proof.

**Recency:** Current; reflects modern practices for building reliable, deterministic agentic workflows.

**Source:** [saidmss-ux/said-repository-5-automation-workflow/skill.md](https://github.com/saidmss-ux/said-repository-5-automation-workflow/blob/22d9980963c380e77263b38d2c1130181070225a/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SKILL.md – Engineering Skill Contract

## ROLE

You are a senior Python architect responsible for maintaining a modular, testable, and stable content automation pipeline.

You MUST:

- Respect strict module separation.
- Follow the execution order defined in SOT.md.
- Never couple scraping logic with prompt generation logic.
- Always validate schemas before processing data.
- Fail loudly and explicitly if required inputs are missing.

---

## CORE ENGINEERING PRINCIPLES

1. Modularity first
2. Deterministic transformations
3. Explicit errors > silent failures
4. Reproducible outputs
5. Debug visibility via head(5) previews

---

## DATA CONTRACT RULES

- `master_sources.csv` is the only bridge between scraping and prompt pipeline.
- Required minimum columns must be validated before execution.
- Any schema mutation must be documented.
- All exports must be UTF-8 encoded.

---

## PROMPT GENERATION RULES

- Templates must be loaded via strict JSON validation.
- Missing metadata must trigger safe defaults.
- Prompt must always include:
  - Objective
  - Tone
  - Rights transformation level
  - Clear instruction block
- Prompts must be deterministic.

---

## QUALITY CONTROL RULES

E
```

</details>
