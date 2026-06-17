---
name: HoangNguyen0403__agent-skills-standard__skill
source: https://github.com/HoangNguyen0403/agent-skills-standard/blob/1a96c1b5c9a236e502dc94d060f488746c2e8db4/skills/typescript/typescript-security/SKILL.md
repo: HoangNguyen0403/agent-skills-standard
kind: skill
stars: 506
last_pushed: 2026-06-14T12:59:34Z
license: apache-2.0
score: 8
domains: [security, web-development, typescript]
tags: [typescript, security, auth, validation]
curated: 2026-06-15
curated_by: config-scout
---

# HoangNguyen0403/agent-skills-standard — skill

**Why it's worth keeping:** It includes highly specific library recommendations (Zod, Argon2id) and actionable anti-patterns like shell interpolation to prevent command injection. The inclusion of a 'Verification' step using LSP diagnostics is an excellent technique for agent accuracy.

**Summary:** Provides high-priority security guidelines for TypeScript development, focusing on input validation, injection prevention, and authentication patterns.

**Source credibility:** High; the source repository has strong social proof with 506 stars and recent activity.

**Recency:** 

**Source:** [HoangNguyen0403/agent-skills-standard/skills/typescript/typescript-security/SKILL.md](https://github.com/HoangNguyen0403/agent-skills-standard/blob/1a96c1b5c9a236e502dc94d060f488746c2e8db4/skills/typescript/typescript-security/SKILL.md) · 506★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: typescript-security
description: Validate input, secure auth tokens, and prevent injection attacks in TypeScript. Use when validating input, handling auth tokens, sanitizing data, or managing secrets and sensitive configuration.
metadata:
  triggers:
    files:
    - '**/*.ts'
    - '**/*.tsx'
    keywords:
    - validate
    - sanitize
    - xss
    - injection
    - auth
    - password
    - secret
    - token
---
# TypeScript Security

## **Priority: P0 (CRITICAL)**

## Validate Input at Boundaries

- Use **`Zod`**, **`Joi`**, or **`class-validator`** at **API boundary**. Always **`parse`** and validate **`user-controlled input`** before using. Use **`safeParse`** for error handling without throwing. Return **`400 with structured errors`** on failure.

See [references/REFERENCE.md](references/REFERENCE.md) for Zod validation schemas, secure cookie setup, and JWT auth patterns.

## Prevent Injection and XSS

- **Sanitization**: Use **`DOMPurify`** for HTML sanitization to prevent **Cross-Site Scripting (XSS)**.
- **SQL Injection**: Use **Parameterized Queries** (e.g., **`pool.query('... WHERE id = $1', [id])`**) or **Type-safe ORMs** (**`Prisma`**/`TypeORM`). Use **`Pri
```

</details>
