---
name: ansible-community__ai-forge__skill
source: https://github.com/ansible-community/ai-forge/blob/036c523a2db455377a89946f089f50611a13390f/cloud_content/module/skills/aws-terminator-implement/SKILL.md
repo: ansible-community/ai-forge
kind: skill
stars: 16
last_pushed: 2026-06-11T15:23:18Z
license: gpl-3.0
score: 8
domains: [infrastructure-as-code, cli-tools, automation]
tags: [aws, ansible, workflow-orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# ansible-community/ai-forge — skill

**Why it's worth keeping:** Provides an excellent blueprint for high-complexity skills by including environment setup, branching logic, multi-step implementation (code + permissions), and automated validation via tox/syntax checks.

**Summary:** Automates a full-lifecycle development workflow for implementing AWS resource terminators and IAM permissions within a specific repository structure.

**Source credibility:** High; part of an active Ansible community repository specializing in AI orchestration.

**Recency:** Current; reflects modern agentic workflows involving tool-chain integration.

**Source:** [ansible-community/ai-forge/cloud_content/module/skills/aws-terminator-implement/SKILL.md](https://github.com/ansible-community/ai-forge/blob/036c523a2db455377a89946f089f50611a13390f/cloud_content/module/skills/aws-terminator-implement/SKILL.md) · 16★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: aws-terminator-implement
description: >-
  Use this skill when implementing terminator classes and IAM permissions in
  the mattclay/aws-terminator repository after analysis. Creates terminator
  class code following Terminator/DbTerminator patterns, generates IAM
  permission blocks, and validates changes for PR submission. Invoke for
  "implement terminator", "create terminator classes", or "add terminator
  permissions".
allowed-tools: Read Edit Write Bash(command:git *) Bash(command:gh *) Bash(command:grep *)
argument-hint: "[--analysis <file>] [--interactive]"
triggers:
  - "implement terminator"
  - "aws-terminator implement"
  - "create terminator classes"
  - "add terminator permissions"
user-invocable: true
---

# AWS Terminator Implement

Implements terminator classes and IAM permissions in the mattclay/aws-terminator repository based on analysis from `/aws-terminator-analyze` or manual specification.

## Purpose

After analyzing an Ansible collection PR with `/aws-terminator-analyze`, this skill:

1. Creates terminator class implementations in the appropriate file
2. Adds IAM permissions to the appropriate policy file
3. Follows aws-terminator patterns and conv
```

</details>
