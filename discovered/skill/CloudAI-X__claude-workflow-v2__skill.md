---
name: CloudAI-X__claude-workflow-v2__skill
source: https://github.com/CloudAI-X/claude-workflow-v2/blob/4c242af16f8a96dfddfee3d07073454bebf92704/skills/security-patterns/SKILL.md
repo: CloudAI-X/claude-workflow-v2
kind: skill
stars: 1369
last_pushed: 2026-06-09T12:15:11Z
license: mit
score: 9
domains: [backend-api, security, web-development]
tags: [auth, jwt, rbac, encryption, best-practices]
curated: 2026-06-15
curated_by: config-scout
---

# CloudAI-X/claude-workflow-v2 — skill

**Why it's worth keeping:** The 'WRONG vs CORRECT' annotations provide high-signal guidance for avoiding common vulnerabilities. The inclusion of an implementation checklist is perfect for maintaining state in long agentic workflows.

**Summary:** A comprehensive security implementation guide that includes authentication, authorization, and secrets management patterns. It features a structured checklist for task tracking.

**Source credibility:** High; highly starred (1300+) and actively maintained repository.

**Recency:** Current; utilizes modern standards like NIST password guidelines and secure JWT/session management.

**Source:** [CloudAI-X/claude-workflow-v2/skills/security-patterns/SKILL.md](https://github.com/CloudAI-X/claude-workflow-v2/blob/4c242af16f8a96dfddfee3d07073454bebf92704/skills/security-patterns/SKILL.md) · 1369★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: security-patterns
description: Implements authentication, authorization, encryption, secrets management, and security hardening patterns. Use when designing auth flows, managing secrets, configuring CORS, implementing rate limiting, or when asked about JWT, OAuth, password hashing, API keys, RBAC, or security best practices.
---

# Security Patterns

### When to Load

- **Trigger**: Auth flows, encryption, secrets management, CORS configuration, input validation, rate limiting
- **Skip**: No security surface involved in the current task

## Security Implementation Workflow

Copy this checklist and track progress:

```
Security Implementation Progress:
- [ ] Step 1: Choose authentication strategy
- [ ] Step 2: Implement authorization model
- [ ] Step 3: Set up password hashing
- [ ] Step 4: Configure secrets management
- [ ] Step 5: Enable encryption (transit + rest)
- [ ] Step 6: Configure CORS
- [ ] Step 7: Add rate limiting
- [ ] Step 8: Validate against anti-patterns checklist
```

## Authentication Patterns

### JWT (JSON Web Tokens)

```typescript
import jwt from "jsonwebtoken";

function generateTokens(user: User) {
  const accessToken = jwt.sign(
    { sub: user.id
```

</details>
