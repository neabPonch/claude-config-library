---
name: mattnigh__skills_collection__profpowell-project-template-claude-skills-authentication-skill
source: https://github.com/mattnigh/skills_collection/blob/adf1a27eb51d9278eeb84d556fbccd56531cf34b/collection/ProfPowell__project-template__claude__skills__authentication__SKILL.md
repo: mattnigh/skills_collection
kind: skill
stars: 23
last_pushed: 2025-12-31T03:21:29Z
license: unknown
score: 8
domains: [backend-api, security]
tags: [authentication, jwt, security, nodejs]
curated: 2026-06-16
curated_by: config-scout
---

# mattnigh/skills_collection — skill

**Why it's worth keeping:** Includes specific security-hardened configurations like exact Argon2 parameters and cookie flags that prevent common implementation errors.

**Summary:** A comprehensive blueprint for implementing complete authentication systems including JWT, Argon2 password hashing, and secure session management.

**Source credibility:** Decent; part of a curated collection of utility patterns rather than generic documentation.

**Recency:** Current; utilizes modern industry standards for token handling and password hashing.

**Source:** [mattnigh/skills_collection/collection/ProfPowell__project-template__claude__skills__authentication__SKILL.md](https://github.com/mattnigh/skills_collection/blob/adf1a27eb51d9278eeb84d556fbccd56531cf34b/collection/ProfPowell__project-template__claude__skills__authentication__SKILL.md) · 23★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: authentication
description: Implement secure authentication with JWT, sessions, OAuth, and password hashing. Use when adding login/logout, token auth, or integrating OAuth providers.
allowed-tools: Read, Write, Edit, Glob, Grep
---

# Authentication Skill

Implement secure authentication patterns for web applications including JWT tokens, sessions, OAuth, and password handling.

---

## When to Use

- Adding login/logout functionality
- Implementing token-based authentication
- Integrating OAuth providers
- Handling password hashing and reset
- Managing sessions and cookies

---

## JWT Authentication

### Token Generation

```javascript
import jwt from 'jsonwebtoken';
import { config } from '../config/index.js';

/**
 * Generate JWT access token
 * @param {object} payload - Token payload (user data)
 * @returns {string} - Signed JWT token
 */
export function generateAccessToken(payload) {
  return jwt.sign(payload, config.jwt.secret, {
    expiresIn: config.jwt.accessExpiresIn || '15m',
    issuer: config.jwt.issuer
  });
}

/**
 * Generate refresh token (longer-lived)
 * @param {object} payload - Token payload
 * @returns {string} - Signed refresh token
 */
export funct
```

</details>
