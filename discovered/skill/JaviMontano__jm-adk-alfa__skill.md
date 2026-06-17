---
name: JaviMontano__jm-adk-alfa__skill
source: https://github.com/JaviMontano/jm-adk-alfa/blob/4a44e90b17d3d38ea3d257801e49158e9af3c3e5/skills/linting-formatting/SKILL.md
repo: JaviMontano/jm-adk-alfa
kind: skill
stars: 2
last_pushed: 2026-06-11T21:22:57Z
license: mit
score: 7
domains: [web-frontend, devops, cli-tools]
tags: [linting, formatting, eslint, quality-assurance]
curated: 2026-06-14
curated_by: config-scout
---

# JaviMontano/jm-adk-alfa — skill

**Why it's worth keeping:** Uses a highly structured 'Discover-Analyze-Execute-Validate' methodology; includes high-value anti-patterns like avoiding auto-fixes in CI to ensure developer awareness.

**Summary:** Provides an end-to-end workflow for setting up automated code quality through linting, formatting, and pre-commit hooks.

**Source credibility:** Low star count (2) but appears to be an individual's specialized toolkit/ADK.

**Recency:** Very recent, following current modern web development standards.

**Source:** [JaviMontano/jm-adk-alfa/skills/linting-formatting/SKILL.md](https://github.com/JaviMontano/jm-adk-alfa/blob/4a44e90b17d3d38ea3d257801e49158e9af3c3e5/skills/linting-formatting/SKILL.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: linting-formatting
author: JM Labs (Javier Montaño)
version: 1.0.0
description: >
  Configure ESLint, Prettier, and Stylelint for automated code quality
  enforcement with pre-commit hooks and CI integration. [EXPLICIT]
  Trigger: "ESLint", "Prettier", "linting", "code formatting", "Stylelint"
allowed-tools:
  - Read
  - Write
  - Glob
  - Grep
  - Bash
---

# Linting & Formatting

> "Arguing about code style in reviews is a waste of time — let the machines decide." — Unknown

## TL;DR

Guides the setup of automated code quality tools — ESLint for code correctness, Prettier for formatting, Stylelint for CSS, pre-commit hooks with Husky/lint-staged, and CI integration. Use when establishing or improving code quality tooling for a project. [EXPLICIT]

## Procedure

### Step 1: Discover
- Check existing linting/formatting configuration files
- Review `package.json` for installed lint/format dependencies
- Identify IDE integration setup (VS Code extensions, settings)
- Check for pre-commit hooks (Husky, pre-commit)

### Step 2: Analyze
- Evaluate ESLint config: which preset (airbnb, standard, recommended)?
- Determine Prettier preferences (semi, single quotes, tab width, trai
```

</details>
