---
name: sipyourdrink-ltd__bernstein__skill
source: https://github.com/sipyourdrink-ltd/bernstein/blob/ef8b8f8c9ef12a3c6a723eeb8af948a49a5b472c/packages/cursor-plugin/skills/bernstein-plan/SKILL.md
repo: sipyourdrink-ltd/bernstein
kind: skill
stars: 574
last_pushed: 2026-06-15T12:23:25Z
license: apache-2.0
score: 8
domains: [agents-ai, cli-tools, orchestration]
tags: [planning, task-decomposition, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# sipyourdrink-ltd/bernstein — skill

**Why it's worth keeping:** The YAML structure using 'role', 'scope', and 'complexity' is an excellent way to formalize task decomposition that can be used across different agentic workflows.

**Summary:** Provides a structured schema for decomposing complex goals into stage-based execution plans with explicit roles and dependencies.

**Source credibility:** Strong; 574 stars and active maintenance indicate a legitimate tool for audit-grade orchestration.

**Recency:** Current; designed specifically for modern CLI agents like Claude Code.

**Source:** [sipyourdrink-ltd/bernstein/packages/cursor-plugin/skills/bernstein-plan/SKILL.md](https://github.com/sipyourdrink-ltd/bernstein/blob/ef8b8f8c9ef12a3c6a723eeb8af948a49a5b472c/packages/cursor-plugin/skills/bernstein-plan/SKILL.md) · 574★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: bernstein-plan
description: >
  Create and manage multi-step execution plans in Bernstein. Plans decompose
  complex goals into stages with dependencies. Use when the user wants to
  plan a complex feature, break down a large task, or review an execution plan
  before agents start working.
---

# Bernstein Plan Mode

Create structured execution plans that get human approval before agents start.

## When to Use

- User describes a complex feature: "implement user authentication with OAuth"
- User wants to break down a large task into stages
- User says "plan this out" or "create a plan for..."
- User wants to review what agents will do before they start

## Instructions

### Creating a plan

1. Analyze the user's request and decompose it into stages and tasks.
2. Write a plan YAML file using this structure:

```yaml
name: "{descriptive plan name}"
description: "{what this plan achieves}"
stages:
  - name: foundation
    steps:
      - goal: "Create database models for user and session"
        role: backend
        scope: small
        complexity: low
      - goal: "Add migration scripts"
        role: backend
        scope: tiny

  - name: implementation
    depends_on: [
```

</details>
