---
name: hoangsonww__JWT-Module
source: https://github.com/hoangsonww/JWT-Module/blob/caea4805f4419be6658e667aca40a290d45fdc18/CLAUDE.md
repo: hoangsonww/JWT-Module
kind: claude-md
stars: 10
last_pushed: 2026-06-05T05:01:02Z
license: mit
score: 8
domains: [backend-api, security, typescript]
tags: [authentication, express, jwt]
curated: 2026-06-14
curated_by: config-scout
---

# hoangsonww/JWT-Module — claude-md

**Why it's worth keeping:** Includes specific procedural workflows (e.g., adding error codes) and explicit instructions for test isolation to prevent state leakage.

**Summary:** Provides structural context and enforces strict architectural/testing constraints for a TypeScript JWT service.

**Source credibility:** Small standalone module with moderate star count; highly structured logic.

**Recency:** Current; uses standard modern TypeScript/Node patterns.

**Source:** [hoangsonww/JWT-Module/CLAUDE.md](https://github.com/hoangsonww/JWT-Module/blob/caea4805f4419be6658e667aca40a290d45fdc18/CLAUDE.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# jwt-module

JWT authentication module built with Express and TypeScript. In-memory storage — no database.

## Key Files

- `src/auth/auth-service.ts` — Core auth logic: register, login, refresh, logout, password change, email update, account delete
- `src/auth/token.ts` — JWT generation, verification, revocation blacklist
- `src/auth/password.ts` — bcrypt hashing (12 rounds), password strength validation
- `src/auth/errors.ts` — `AuthError` class, `AuthErrorCode` union type
- `src/auth/types.ts` — Shared interfaces: `User`, `AuthTokens`, `TokenPayload`, `RegisterInput`, `LoginInput`
- `src/api/app.ts` — Express app factory, `AuthService` interface
- `src/api/auth-router.ts` — Route handlers, `ERROR_STATUS_MAP` for error-to-status mapping
- `src/api/middleware.ts` — `authenticateToken` middleware, request logger
- `src/api/rate-limiter.ts` — Per-IP sliding window rate limiter
- `src/api/validation.ts` — Zod schemas for request body validation
- `src/server.ts` — Entry point, wires auth-service into Express app

## Commands

- Build: `npm run build`
- Test: `npm test`
- Test with coverage: `npm run test:coverage`
- Dev server: `PORT=5001 npx ts-node src/server.ts`

## Important Pat
```

</details>
