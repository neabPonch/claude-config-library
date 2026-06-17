---
name: martinholovsky__claude-skills-generator__skill
source: https://github.com/martinholovsky/claude-skills-generator/blob/1086ef25672acba2916220c6ce032a612cd9dc98/skills/fastapi/SKILL.md
repo: martinholovsky/claude-skills-generator
kind: skill
stars: 39
last_pushed: 2025-12-06T21:40:03Z
license: unlicense
score: 9
domains: [backend-api, security]
tags: [fastapi, python, rest-api, security-first]
curated: 2026-06-15
curated_by: config-scout
---

# martinholovsky/claude-skills-generator — skill

**Why it's worth keeping:** It features a unique 'Validation Gate' linking specific CVEs to version requirements and provides hardened implementation patterns for high-risk tasks like file uploads and CORS.

**Summary:** A security-hardened FastAPI development skill that prioritizes production-ready patterns and proactive vulnerability mitigation.

**Source credibility:** The inclusion of very recent 2024 CVEs suggests high-quality, manual curation by an expert developer.

**Recency:** Extremely current; uses up-to-date security considerations and library versions from late 2024/early 2025.

**Source:** [martinholovsky/claude-skills-generator/skills/fastapi/SKILL.md](https://github.com/martinholovsky/claude-skills-generator/blob/1086ef25672acba2916220c6ce032a612cd9dc98/skills/fastapi/SKILL.md) · 39★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: fastapi
description: REST API and WebSocket development with FastAPI emphasizing security, performance, and async patterns
model: sonnet
risk_level: HIGH
---

# FastAPI Development Skill

## File Organization

- **SKILL.md**: Core principles, patterns, essential security (this file)
- **references/security-examples.md**: CVE details and OWASP implementations
- **references/advanced-patterns.md**: Advanced FastAPI patterns
- **references/threat-model.md**: Attack scenarios and STRIDE analysis

## Validation Gates

### Gate 0.2: Vulnerability Research (BLOCKING for HIGH-RISK)
- **Status**: PASSED (5+ CVEs documented)
- **Research Date**: 2025-11-20
- **CVEs**: CVE-2024-47874, CVE-2024-12868, CVE-2023-30798, Starlette DoS variants

---

## 1. Overview

**Risk Level**: HIGH

**Justification**: FastAPI applications handle authentication, database access, file uploads, and external API communication. DoS vulnerabilities in Starlette, injection risks, and improper validation can compromise availability and security.

You are an expert FastAPI developer creating secure, performant REST APIs and WebSocket services. You configure proper validation, authentication, and security head
```

</details>
