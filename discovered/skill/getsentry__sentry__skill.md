---
name: getsentry__sentry__skill
source: https://github.com/getsentry/sentry/blob/67c07745163f07358b9454b60d4fe692d3ea5116/.agents/skills/sentry-security/SKILL.md
repo: getsentry/sentry
kind: skill
stars: 44105
last_pushed: 2026-06-16T04:17:21Z
license: other
score: 9
domains: [backend-api, security, python]
tags: [security-audit, idor-detection, code-review, pattern-matching]
curated: 2026-06-16
curated_by: config-scout
---

# getsentry/sentry — skill

**Why it's worth keeping:** Replaces generic OWASP theory with specific 'Red Flag' code snippets and a rigorous multi-layer enforcement tracing protocol to reduce false positives.

**Summary:** A domain-aware security review skill that uses historical vulnerability patterns to detect IDOR, privilege escalation, and injection specifically within Sentry's architecture.

**Source credibility:** Extremely high; sourced from Sentry, a major industry-standard security and monitoring platform.

**Recency:** Very current; documentation explicitly references security patches from the last year.

**Source:** [getsentry/sentry/.agents/skills/sentry-security/SKILL.md](https://github.com/getsentry/sentry/blob/67c07745163f07358b9454b60d4fe692d3ea5116/.agents/skills/sentry-security/SKILL.md) · 44105★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: sentry-security
description: 'Sentry-specific security review based on real vulnerability history. Use when reviewing Sentry endpoints, serializers, or views for security issues. Trigger keywords: "sentry security review", "check for IDOR", "access control review", "org scoping", "cross-org", "security audit endpoint".'
allowed-tools: Read Grep Glob Bash
---

# Sentry Security Review

Find security vulnerabilities in Sentry code by checking for the patterns that have caused real vulnerabilities in this codebase.

This skill is Sentry-specific. It encodes patterns from 37 real security patches shipped in the last year — not generic OWASP theory.

## Scope

Review the code provided by the user (file, diff, or endpoint). Research the codebase as needed to build confidence before reporting.

Report only **HIGH** and **MEDIUM** confidence findings. Do not report theoretical issues.

| Confidence | Criteria                                   | Action                       |
| ---------- | ------------------------------------------ | ---------------------------- |
| **HIGH**   | Traced the flow, confirmed no check exists | Report with fix              |
| **MEDIUM** | Check may e
```

</details>
