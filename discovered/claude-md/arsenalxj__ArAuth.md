---
name: arsenalxj__ArAuth
source: https://github.com/arsenalxj/ArAuth/blob/bb34168f510fc9fdb226ddcc05885877f9b41699/CLAUDE.md
repo: arsenalxj/ArAuth
kind: claude-md
stars: 0
last_pushed: 2026-04-28T13:01:43Z
license: unknown
score: 9
domains: [backend-api, security, mobile-sdk]
tags: [auth, cloudflare-workers, flutter, d1, security]
curated: 2026-06-16
curated_by: config-scout
---

# arsenalxj/ArAuth — claude-md

**Why it's worth keeping:** Includes exact 'wrangler' commands for database migrations and provides explicit implementation details for security patterns (PBKDF2/JWT) to prevent insecure AI-generated suggestions.

**Summary:** A highly detailed technical specification that bridges a Cloudflare Worker backend with a Flutter SDK, covering architecture, schema, and security protocols.

**Source credibility:** Low star count, but the depth of technical detail suggests a functional, real-world authentication system.

**Recency:** Current; aligns with modern Cloudflare Wrangler development workflows.

**Source:** [arsenalxj/ArAuth/CLAUDE.md](https://github.com/arsenalxj/ArAuth/blob/bb34168f510fc9fdb226ddcc05885877f9b41699/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Layout

```
auth-worker/   Cloudflare Worker — auth API + admin dashboard
ar_auth/       Flutter Dart SDK package
docs/DanDan/   Design spec (plan.md, ui-preview.html)
```

## auth-worker Commands

All commands run from `auth-worker/`:

```bash
npm install          # install deps (first time)
npx wrangler dev     # local dev (uses local D1)
npx wrangler deploy  # deploy to production
npx wrangler d1 execute auth-db --remote --file=migrations/0001_initial.sql  # 初始建表
npx wrangler d1 execute auth-db --remote --file=migrations/0002_users_integer_id.sql  # users.id 改为自增整数
npx wrangler d1 execute auth-db --remote --file=migrations/0003_sessions.sql  # 新增 v2 session 表
```

本地运行 `wrangler dev` 时需要在 `auth-worker/.dev.vars` 中提供：

```bash
JWT_SECRET=your-local-dev-secret
```

## Architecture

### auth-worker (Hono + Cloudflare D1)

Single Worker serving two concerns:

**Auth API** — 同时提供 `v1` 与 `v2`
- All routes require `X-App-Key` / `X-App-Secret` headers (verified by `middleware/app-auth.ts`)
- Rate limited per IP (`middleware/rate-limit.ts`, in-memory, resets
```

</details>
