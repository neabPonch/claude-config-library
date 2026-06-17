---
name: rohitg00__awesome-claude-code-toolkit__skill
source: https://github.com/rohitg00/awesome-claude-code-toolkit/blob/ebdf1d596d2cde5c5cceb32177e8d1cf4829e7d9/skills/authentication-patterns/SKILL.md
repo: rohitg00/awesome-claude-code-toolkit
kind: skill
stars: 2058
last_pushed: 2026-05-12T07:18:34Z
license: apache-2.0
score: 8
domains: [backend-api, security]
tags: [auth, jwt, oauth2, rbac]
curated: 2026-06-15
curated_by: config-scout
---

# rohitg00/awesome-claude-code-toolkit — skill

**Why it's worth keeping:** Includes specific security-critical logic like PKCE code challenge generation and a practical anti-pattern/checklist guide.

**Summary:** Provides structured implementation patterns for JWT lifecycles, OAuth2 with PKCE, and RBAC-based authorization.

**Source credibility:** High community trust indicated by 2000+ stars and recent maintenance.

**Recency:** Uses modern industry standards including PKCE and short-lived token rotation.

**Source:** [rohitg00/awesome-claude-code-toolkit/skills/authentication-patterns/SKILL.md](https://github.com/rohitg00/awesome-claude-code-toolkit/blob/ebdf1d596d2cde5c5cceb32177e8d1cf4829e7d9/skills/authentication-patterns/SKILL.md) · 2058★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: authentication-patterns
description: Authentication and authorization patterns including OAuth2, JWT, RBAC, session management, and PKCE flows
---

# Authentication Patterns

## JWT Access and Refresh Tokens

```typescript
import jwt from "jsonwebtoken";

interface TokenPayload {
  sub: string;
  email: string;
  roles: string[];
}

function generateTokens(user: User) {
  const accessToken = jwt.sign(
    { sub: user.id, email: user.email, roles: user.roles },
    process.env.JWT_SECRET!,
    { expiresIn: "15m", issuer: "auth-service" }
  );

  const refreshToken = jwt.sign(
    { sub: user.id, tokenVersion: user.tokenVersion },
    process.env.REFRESH_SECRET!,
    { expiresIn: "7d", issuer: "auth-service" }
  );

  return { accessToken, refreshToken };
}

function verifyAccessToken(token: string): TokenPayload {
  return jwt.verify(token, process.env.JWT_SECRET!, {
    issuer: "auth-service",
  }) as TokenPayload;
}
```

Short-lived access tokens (15 minutes) with longer-lived refresh tokens (7 days). Store refresh tokens in HTTP-only cookies.

## Auth Middleware

```typescript
function authenticate(req: Request, res: Response, next: NextFunction) {
  const header = req.
```

</details>
