---
name: duriantaco__skylos__skill
source: https://github.com/duriantaco/skylos/blob/92431bc4d360d402e8a61aceacc5500780e1e83b/.claude/skills/skylos/SKILL.md
repo: duriantaco/skylos
kind: skill
stars: 453
last_pushed: 2026-06-14T03:22:58Z
license: apache-2.0
score: 8
domains: [cli-tools, security, devops]
tags: [cli, static-analysis, security-scanner]
curated: 2026-06-14
curated_by: config-scout
---

# duriantaco/skylos — skill

**Why it's worth keeping:** It uses a 'Reference-based' pattern to reduce context bloat and includes highly specific command defaults that prevent agent guesswork during JSON parsing or tool execution.

**Summary:** This file provides specialized operational instructions for interacting with the Skylos CLI, including navigation-based context management and specific command templates.

**Source credibility:** High; the source repository is active and well-regarded within its niche with significant star count.

**Recency:** Current; it follows modern agentic patterns for safe CLI interaction and context minimization.

**Source:** [duriantaco/skylos/.claude/skills/skylos/SKILL.md](https://github.com/duriantaco/skylos/blob/92431bc4d360d402e8a61aceacc5500780e1e83b/.claude/skills/skylos/SKILL.md) · 453★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: skylos
description: >-
  Run, interpret, or modify Skylos safely. Use when the user asks to scan code
  with Skylos, explain SKY-* findings, triage dead-code false positives, audit
  security/secrets/SCA/LLM behavior, update Skylos rules/docs/CI, benchmark
  analyzer behavior, or change this repository safely.
---

# Skylos

Use this skill to work with Skylos without rediscovering the CLI, output shape,
test surface, and security guardrails.

## Choose The Reference

- Running Skylos, choosing output formats, parsing JSON, filtering, gates, and
  install troubleshooting: read `references/cli.md`.
- Changing Skylos code, adding rules, updating docs, selecting focused tests,
  or preserving repo hygiene: read `references/repo-workflow.md`.
- Basic security scan usage, secrets, and SCA: read `references/security.md`.
  For scanner bypasses, LLM evidence filters, cloud/CI policy, or severity
  classification, use `/skylos-security`.
- Dead-code false positives, framework liveness, runtime tracing, Vulture
  comparisons, and benchmark work: read `references/dead-code.md`.
- GitHub Actions, SARIF, repo map Pages, CI gates, docs deploy, and generated
  workflows: read `reference
```

</details>
