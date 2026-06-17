---
name: jeremylongshore__claude-code-plugins-plus-skills__skill
source: https://github.com/jeremylongshore/claude-code-plugins-plus-skills/blob/57b5254bd3d6c39f2d15f3d9750db89b3801d8ab/plugins/saas-packs/sentry-pack/skills/sentry-known-pitfalls/SKILL.md
repo: jeremylongshore/claude-code-plugins-plus-skills
kind: skill
stars: 2385
last_pushed: 2026-06-16T02:04:01Z
license: mit
score: 9
domains: [observability, devops, web-development]
tags: [sentry, debugging, audit, error-tracking]
curated: 2026-06-16
curated_by: config-scout
---

# jeremylongshore/claude-code-plugins-plus-skills — skill

**Why it's worth keeping:** It provides actionable shell one-liners for codebase detection and a highly transferable 'Wrong vs Right' pattern for refactoring code.

**Summary:** A diagnostic playbook that uses specific grep commands to audit Sentry SDK configurations for production issues like data loss and cost overruns. It includes proactive scanning steps followed by clear remediation patterns.

**Source credibility:** High; part of a large, highly starred, and actively maintained open-source skill repository.

**Recency:** Current; updated with the latest Sentry SDK 8.x standards.

**Source:** [jeremylongshore/claude-code-plugins-plus-skills/plugins/saas-packs/sentry-pack/skills/sentry-known-pitfalls/SKILL.md](https://github.com/jeremylongshore/claude-code-plugins-plus-skills/blob/57b5254bd3d6c39f2d15f3d9750db89b3801d8ab/plugins/saas-packs/sentry-pack/skills/sentry-known-pitfalls/SKILL.md) · 2385★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: sentry-known-pitfalls
description: 'Identify and fix common Sentry SDK pitfalls that cause silent data loss,

  cost overruns, and missed alerts. Covers 10 anti-patterns with fix code.

  Use when auditing Sentry config, debugging missing events, or reviewing

  SDK setup. Trigger: "sentry pitfalls", "sentry anti-patterns",

  "sentry mistakes", "why are sentry events missing".

  '
allowed-tools: Read, Write, Edit, Grep, Glob, Bash(node:*), Bash(npm:*), Bash(npx:*),
  Bash(grep:*), Bash(find:*)
version: 1.0.0
license: MIT
author: Jeremy Longshore <jeremy@intentsolutions.io>
tags:
- saas
- sentry
- anti-patterns
- troubleshooting
- best-practices
- sdk
- configuration
compatibility: Designed for Claude Code, also compatible with Codex and OpenClaw
---
# Sentry Known Pitfalls

## Overview

Ten production-grade Sentry SDK anti-patterns that silently break error tracking, inflate costs, or leave teams blind to failures. Each pitfall includes the broken pattern, root cause, and production-ready fix.

For extended code samples and audit scripts, see [configuration pitfalls](references/configuration-pitfalls.md), [error capture pitfalls](references/error-capture-pitfalls.md), [
```

</details>
