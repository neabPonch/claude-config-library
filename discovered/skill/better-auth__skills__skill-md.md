---
name: better-auth__skills__skill-md
source: https://github.com/better-auth/skills/blob/6a1636950a1d7fc53602639ce7505a4a5d39c797/security/SKILL.MD
repo: better-auth/skills
kind: skill
stars: 197
last_pushed: 2026-03-02T09:11:17Z
license: unknown
score: 9
domains: [security, backend-api, web-development]
tags: [auth, typescript, security-best-practices, rate-limiting]
curated: 2026-06-14
curated_by: config-scout
---

# better-auth/skills — skill

**Why it's worth keeping:** Provides highly actionable code snippets for advanced security patterns like database auditing hooks, per-endpoint rate limiting, and serverless background task integration.

**Summary:** A comprehensive technical blueprint for securing a Better Auth implementation through specific configuration patterns.

**Source credibility:** High; the documentation is derived from the official 'better-auth' ecosystem.

**Recency:** Very recent; last updated 3 months ago, ensuring compatibility with modern TypeScript/Node environments.

**Source:** [better-auth/skills/security/SKILL.MD](https://github.com/better-auth/skills/blob/6a1636950a1d7fc53602639ce7505a4a5d39c797/security/SKILL.MD) · 197★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: better-auth-security-best-practices
description: Configure rate limiting, manage auth secrets, set up CSRF protection, define trusted origins, secure sessions and cookies, encrypt OAuth tokens, track IP addresses, and implement audit logging for Better Auth. Use when users need to secure their auth setup, prevent brute force attacks, or harden a Better Auth deployment.
---

## Secret Management

### Configuring the Secret

```ts
import { betterAuth } from "better-auth";

export const auth = betterAuth({
  secret: process.env.BETTER_AUTH_SECRET, // or via `BETTER_AUTH_SECRET` env
});
```

Better Auth looks for secrets in this order:
1. `options.secret` in your config
2. `BETTER_AUTH_SECRET` environment variable
3. `AUTH_SECRET` environment variable

### Secret Requirements

- Rejects default/placeholder secrets in production
- Warns if shorter than 32 characters or entropy below 120 bits
- Generate: `openssl rand -base64 32`
- Never commit secrets to version control

## Rate Limiting

Enabled in production by default. Applies to all endpoints. Plugins can override per-endpoint.

### Default Configuration

```ts
import { betterAuth } from "better-auth";

export const auth =
```

</details>
