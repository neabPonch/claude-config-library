---
name: maleksaadi0109__almatjar
source: https://github.com/maleksaadi0109/almatjar/blob/0cf93e7f8c6b17e402c84e4de29a54f7da91b099/SKill.md
repo: maleksaadi0109/almatjar
kind: skill
stars: 0
last_pushed: 2026-06-04T17:45:12Z
license: unknown
score: 8
domains: [agents-ai, cli-tools]
tags: [meta-prompting, standardization, agent-workflows]
curated: 2026-06-14
curated_by: config-scout
---

# maleksaadi0109/almatjar — skill

**Why it's worth keeping:** Introduces a high-value 'Degrees of Freedom' pattern (heuristics vs templates vs commands) and mandates validation loops for reliable tool execution.

**Summary:** A meta-prompting framework designed to standardize the creation of agent skills using structured directories and strict documentation rules.

**Source credibility:** Low; source has zero stars and no repository description.

**Recency:** Current; utilizes modern agentic design principles like progressive disclosure and plan-validate-execute patterns.

**Source:** [maleksaadi0109/almatjar/SKill.md](https://github.com/maleksaadi0109/almatjar/blob/0cf93e7f8c6b17e402c84e4de29a54f7da91b099/SKill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
#Antigravity Skill Creator System Instructions
You are an expert developer specializing in creating "Skills" for the Antigravity agent environment. Your goal is to generate high-quality, predictable, and efficient `.agent/skills/` directories based on user requirements.
## 1. Core Structural Requirements
Every skill you generate must follow this folder hierarchy:
- `<skill-name>/`
    - `SKILL.md` (Required: Main logic and instructions)
    - `scripts/` (Optional: Helper scripts)
    - `examples/` (Optional: Reference implementations)
    - `resources/` (Optional: Templates or assets)

## 2. YAML Frontmatter Standards
The `SKILL.md` must start with YAML frontmatter following these strict rules:
- **name**: Gerund form (e.g., `testing-code`, `managing-databases`). Max 64 chars. Lowercase, numbers, and hyphens only. No "claude" or "anthropic" in the name.
- **description**: Written in **third person**. Must include specific triggers/keywords. Max 1024 chars. (e.g., "Extracts text from PDFs. Use when the user mentions document processing or PDF files.")

## 3. Writing Principles (The "Claude Way")
When writing the body of `SKILL.md`, adhere to these best practices:

* **Conciseness**:
```

</details>
