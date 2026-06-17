---
name: FerroxLabs__wayland__skill
source: https://github.com/FerroxLabs/wayland/blob/be93d753f9b5b17c7d5250a83df4826141d29484/src/process/resources/skills-library/bodies/skills/testing-quality/integration-testing-patterns/SKILL.md
repo: FerroxLabs/wayland
kind: skill
stars: 426
last_pushed: 2026-06-15T10:56:49Z
license: agpl-3.0
score: 9
domains: [backend-engineering, devops, software-testing]
tags: [integration-testing, test-automation, decision-frameworks]
curated: 2026-06-15
curated_by: config-scout
---

# FerroxLabs/wayland — skill

**Why it's worth keeping:** The inclusion of a specific 'Decision matrix' for boundary types and detailed tactics for database isolation (rollback vs. schema-per-test) are immediately actionable templates.

**Summary:** A highly structured decision framework for managing integration testing across complex system boundaries. It provides clear heuristics for choosing test doubles and managing state isolation.

**Source credibility:** High; the source repository is well-starred and shows recent, active maintenance.

**Recency:** Current; utilizes modern industry standards like Testcontainers and containerized infrastructure management.

**Source:** [FerroxLabs/wayland/src/process/resources/skills-library/bodies/skills/testing-quality/integration-testing-patterns/SKILL.md](https://github.com/FerroxLabs/wayland/blob/be93d753f9b5b17c7d5250a83df4826141d29484/src/process/resources/skills-library/bodies/skills/testing-quality/integration-testing-patterns/SKILL.md) · 426★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: integration-testing-patterns
description: |
  Guides expert-level integration testing patterns implementation: automation and best-practices decision frameworks, production-ready patterns, and concrete templates for integration testing patterns workflows.
  Use when the user asks about integration testing patterns, integration testing patterns configuration, or testing best practices for integration projects.
  Do NOT use when the user needs a different testing quality capability -- check sibling skills in the testing quality subcategory.
license: Apache-2.0
metadata:
  author: foundry-skills
  version: "1.0.0"
  tags: "testing automation best-practices"
  category: "testing-quality"
  subcategory: "testing-quality"
  depends: ""
  disclaimer: "none"
  difficulty: "intermediate"
---
# Integration Testing Patterns

## When to Use

**Use this skill when:**
- A user wants to design or improve integration tests that verify interactions between two or more real components -- databases, message queues, HTTP APIs, caches, or third-party services
- A user asks how to structure tests that span service boundaries, such as testing a REST endpoint that writes to PostgreSQL and publis
```

</details>
