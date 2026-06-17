---
name: bitsoex__bitso-java__skill
source: https://github.com/bitsoex/bitso-java/blob/7d98e2c384acc60df50ce6ac92168e4cda49da47/.claude/skills/git-hooks/SKILL.md
repo: bitsoex/bitso-java
kind: skill
stars: 38
last_pushed: 2026-03-02T04:41:20Z
license: mit
score: 8
domains: [cli-tools, devops, git]
tags: [git-hooks, automation, workflow-optimization]
curated: 2026-06-16
curated_by: config-scout
---

# bitsoex/bitso-java — skill

**Why it's worth keeping:** The architecture of using an `npm prepare` script to automate the configuration of `core.hooksPath` is a professional-grade pattern. The concept of non-blocking, informative hooks is highly valuable for AI agent interactions and new developer onboarding.

**Summary:** Provides a blueprint for an automated, version-controlled Git hook system that uses symlinks and a bootstrap script. Features a unique 'Informative Mode' designed to warn users without blocking their workflow.

**Source credibility:** Bitso is a recognized crypto exchange; while the repo is specialized, the technical implementation in the file is high-quality.

**Recency:** Modern (requires Node.js 20+).

**Source:** [bitsoex/bitso-java/.claude/skills/git-hooks/SKILL.md](https://github.com/bitsoex/bitso-java/blob/7d98e2c384acc60df50ce6ac92168e4cda49da47/.claude/skills/git-hooks/SKILL.md) · 38★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: git-hooks
description: >
  Set up, validate, and maintain Git hooks (pre-commit, pre-push, etc.) following
  best practices. Ensures hooks are version-controlled, automatically installed,
  and follow consistent patterns across the team. Use when creating new hooks,
  debugging hook issues, or ensuring hook compliance.
compatibility: Requires Node.js 20+; works with any Git repository
metadata:
  version: "2.1"
  targeting:
    include:
      - repo: "bitsoex/ai-code-instructions"
---

# Git Hooks

This skill provides guidance for implementing and maintaining Git hooks that enforce code quality standards before commits and pushes reach the repository.

## When to use this skill

- Setting up Git hooks in a new repository
- Creating new pre-commit or pre-push hooks
- Debugging hook installation or execution issues
- Ensuring hooks follow team standards
- Migrating from manual hooks to version-controlled hooks
- Integrating with existing hook systems (Husky, pre-commit, lefthook)

## Skill Contents

### Sections

- [When to use this skill](#when-to-use-this-skill)
- [Distributed Hooks (Informative Mode)](#distributed-hooks-informative-mode)
- [Assets](#assets)
- [Architectu
```

</details>
