---
name: duckduckgo__apple-browsers__skill
source: https://github.com/duckduckgo/apple-browsers/blob/3724e815d1305d725aae420544f74757259194e4/.claude/skills/ddg-sentry-report/SKILL.md
repo: duckduckgo/apple-browsers
kind: skill
stars: 222
last_pushed: 2026-06-15T07:47:17Z
license: apache-2.0
score: 9
domains: [devops, mobile-dev, agentic-workflows, ci-cd]
tags: [sentry, asana, crash-triage, automation]
curated: 2026-06-15
curated_by: config-scout
---

# duckduckgo/apple-browsers — skill

**Why it's worth keeping:** Uses 'System Truth' (Bash date) to prevent time drift, includes rigorous PII/security sanitization rules, and provides fallback logic for auto-resolving task hierarchies.

**Summary:** Automates Sentry crash triage by querying error data and filing structured subtasks in Asana for Apple-platform releases.

**Source credibility:** High; a production-grade skill from the DuckDuckGo engineering organization.

**Recency:** Extremely current; pushed within the last month.

**Source:** [duckduckgo/apple-browsers/.claude/skills/ddg-sentry-report/SKILL.md](https://github.com/duckduckgo/apple-browsers/blob/3724e815d1305d725aae420544f74757259194e4/.claude/skills/ddg-sentry-report/SKILL.md) · 222★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ddg-sentry-report
description: Invoke ONLY when the user explicitly runs `/ddg-sentry-report` or names this skill by name (e.g. "use ddg-sentry-report for macOS 1.186"). Do NOT auto-invoke from symptom/intent matching — the skill writes to a shared Asana task and must be user-initiated. If the user asks about Sentry issues or crash triage without naming this skill, answer directly. Inputs: project (iOS/macOS) and optional version, release-type, Asana parent URL, and time range — body documents resolution rules.
---

# ddg-sentry-report

## Overview

Produces a structured Sentry crash triage report for a DuckDuckGo Apple release and files it as a new subtask under a parent Asana task. The parent is either supplied by the user as a URL, or auto-resolved from the platform's Weekly Release DRI task → today's "<Weekday> status" subtask. Distinguishes pre-existing issues from new-in-version regressions, sorts by severity, attributes likely authors via git blame (initials + PR links only — never full names).

## Supporting files

- [`references/constants.md`](references/constants.md) — Sentry/Asana GIDs, slugs, project filters, release-string conventions.
- [`templates/main-repo
```

</details>
