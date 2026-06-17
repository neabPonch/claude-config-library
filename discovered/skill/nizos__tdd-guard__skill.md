---
name: nizos__tdd-guard__skill
source: https://github.com/nizos/tdd-guard/blob/73b647f8c4ac43753d61d1063f12b0fab527f050/plugin/skills/setup/SKILL.md
repo: nizos/tdd-guard
kind: skill
stars: 2197
last_pushed: 2026-06-08T14:05:43Z
license: mit
score: 9
domains: [cli-tools, testing, devops]
tags: [tdd, automation, setup-script, configuration]
curated: 2026-06-15
curated_by: config-scout
---

# nizos/tdd-guard — skill

**Why it's worth keeping:** Demonstrates how to provide exact code snippets for various environments while establishing strict safety boundaries to prevent the agent from modifying unrelated project configurations.

**Summary:** A specialized setup skill that automates the installation and configuration of test reporters across diverse ecosystems to enable standardized TDD feedback.

**Source credibility:** High; 2k+ stars and highly active maintenance indicate a widely-used, reliable toolset.

**Recency:** Current; specifically targets the modern Claude Code ecosystem and `.claude` directory structures.

**Source:** [nizos/tdd-guard/plugin/skills/setup/SKILL.md](https://github.com/nizos/tdd-guard/blob/73b647f8c4ac43753d61d1063f12b0fab527f050/plugin/skills/setup/SKILL.md) · 2197★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
description: Set up or update TDD Guard for the current project. Detects the test framework, installs or updates the matching reporter, and configures or migrates its configuration to match the current specification.
disable-model-invocation: true
allowed-tools: [Read, Glob, Grep]
---

# TDD Guard Setup

Set up TDD Guard for the current project. Your goal is to:

1. Identify the test framework(s) used in this project
2. Install the matching TDD Guard reporter, or update it if already present
3. Configure the reporter, or migrate an existing configuration to match the current specification

## Reporter packages

| Framework | Reporter package                                         | Registry   |
| --------- | -------------------------------------------------------- | ---------- |
| Vitest    | tdd-guard-vitest                                         | npm        |
| Jest      | tdd-guard-jest                                           | npm        |
| Storybook | tdd-guard-storybook                                      | npm        |
| pytest    | tdd-guard-pytest                                         | PyPI       |
| PHPUnit   | tdd-guard/phpunit
```

</details>
