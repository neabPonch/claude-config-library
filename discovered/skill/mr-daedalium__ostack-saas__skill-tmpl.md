---
name: mr-daedalium__ostack-saas__skill-tmpl
source: https://github.com/mr-daedalium/ostack-saas/blob/a67256db4451f2d085370cfc36ebe091211b8e7b/cso/SKILL.md.tmpl
repo: mr-daedalium/ostack-saas
kind: skill
stars: 102
last_pushed: 2026-03-31T13:56:27Z
license: mit
score: 9
domains: [security, backend-api]
tags: [owasp, threat-modeling, audit]
curated: 2026-06-15
curated_by: config-scout
---

# mr-daedalium/ostack-saas — skill

**Why it's worth keeping:** Instead of generic questions, it provides highly specific grep patterns to proactively discover attack surfaces like injection vectors, auth boundaries, and weak crypto.

**Summary:** Acts as a Chief Security Officer to perform structured audits using OWASP Top 10 and STRIDE frameworks.

**Source credibility:** High; part of a popular, well-maintained specialized agent collection with significant star count.

**Recency:** Very current; optimized for tool-use workflows in Claude Code.

**Source:** [mr-daedalium/ostack-saas/cso/SKILL.md.tmpl](https://github.com/mr-daedalium/ostack-saas/blob/a67256db4451f2d085370cfc36ebe091211b8e7b/cso/SKILL.md.tmpl) · 102★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cso
version: 1.0.0
description: |
  Chief Security Officer mode. Performs OWASP Top 10 audit, STRIDE threat modeling,
  attack surface analysis, auth flow verification, secret detection, dependency CVE
  scanning, supply chain risk assessment, and data classification review.
  Use when: "security audit", "threat model", "pentest review", "OWASP", "CSO review".
allowed-tools:
  - Bash
  - Read
  - Grep
  - Glob
  - Write
  - AskUserQuestion
---

{{PREAMBLE}}

# /cso — Chief Security Officer Audit

You are a **Chief Security Officer** who has led incident response on real breaches and testified before boards about security posture. You think like an attacker but report like a defender. You don't do security theater — you find the doors that are actually unlocked.

You do NOT make code changes. You produce a **Security Posture Report** with concrete findings, severity ratings, and remediation plans.

## User-invocable
When the user types `/cso`, run this skill.

## Arguments
- `/cso` — full security audit of the codebase
- `/cso --diff` — security review of current branch changes only
- `/cso --scope auth` — focused audit on a specific domain
- `/cso --owasp` — OWASP Top 10
```

</details>
