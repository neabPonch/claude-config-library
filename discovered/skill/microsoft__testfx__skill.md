---
name: microsoft__testfx__skill
source: https://github.com/microsoft/testfx/blob/4aff74ff1ab48074e57705443950dfb31d46b250/.agents/skills/code-testing-agent/SKILL.md
repo: microsoft/testfx
kind: skill
stars: 1020
last_pushed: 2026-06-15T15:47:34Z
license: mit
score: 9
domains: [testing, devops, ai-agents]
tags: [unit-testing, multi-agent, automation, pipeline]
curated: 2026-06-15
curated_by: config-scout
---

# microsoft/testfx — skill

**Why it's worth keeping:** The orchestration patterns—specifically scope-based strategy selection (Direct vs Iterative) and the use of sub-agents for self-correction (Fixer/Linter)—are elite-tier agentic techniques. It also demonstrates excellent state management using a localized directory structure.

**Summary:** Defines a sophisticated multi-agent pipeline for automated unit test generation and verification across diverse languages. It orchestrates specialized roles through a structured Research → Plan → Implement workflow.

**Source credibility:** High; originated from Microsoft's testing platform repository.

**Recency:** Very current, specifically designed for modern agentic workflows and self-correcting loops.

**Source:** [microsoft/testfx/.agents/skills/code-testing-agent/SKILL.md](https://github.com/microsoft/testfx/blob/4aff74ff1ab48074e57705443950dfb31d46b250/.agents/skills/code-testing-agent/SKILL.md) · 1020★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: code-testing-agent
description: >-
  Generates and writes new unit tests for any programming language —
  scaffolds .NET test projects, pytest suites, Vitest/Jest suites,
  Go test files, and JUnit suites, and configures coverage tooling
  (coverlet, pytest-cov, @vitest/coverage-v8) as part of test
  generation. Use when asked to generate tests, generate pytest
  tests, generate Vitest tests, write unit tests, add tests, improve
  coverage, comprehensive tests, or scaffold a new test project or
  suite for an app, service, library, REST API, blueprint, or
  package — including project-wide, multi-file test generation
  across services, repositories, routes, and modules. Supports
  C#/.NET, Python (pytest, Flask/Django), TypeScript/JavaScript
  (Vitest, Jest, Mocha), Go, Rust, Java (JUnit). Runs a research,
  planning, and implementation pipeline so tests compile and pass.
  DO NOT USE FOR: running existing tests (use run-tests); analyzing
  existing coverage reports (use coverage-analysis or crap-score);
  MSTest modernization (use writing-mstest-tests).
license: MIT
---

# Code Testing Generation Skill

An AI-powered skill that generates comprehensive, workable unit test
```

</details>
