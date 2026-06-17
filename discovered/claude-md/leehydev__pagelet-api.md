---
name: leehydev__pagelet-api
source: https://github.com/leehydev/pagelet-api/blob/23598df6eb2de1a75e8fbc65808051ff1983d19a/claude.md
repo: leehydev/pagelet-api
kind: claude-md
stars: 0
last_pushed: 2026-02-07T04:37:29Z
license: unknown
score: 9
domains: [backend-api, nestjs]
tags: [nest-js, typescript, architecture-pattern, api-design]
curated: 2026-06-16
curated_by: config-scout
---

# leehydev/pagelet-api — claude-md

**Why it's worth keeping:** Provides concrete code snippets for complex logic like the 'Controller Separation Pattern' and unique Enum/Entity handling strategies. It eliminates ambiguity by showing exactly how to structure errors, DTOs, and guards.

**Summary:** A highly detailed technical specification for a NestJS multi-tenant API that defines strict architectural rules and implementation patterns.

**Source credibility:** High-density manual documentation suggests a professional developer rather than an automated tool.

**Recency:** Current; uses modern NestJS 11 and TypeScript practices.

**Source:** [leehydev/pagelet-api/claude.md](https://github.com/leehydev/pagelet-api/blob/23598df6eb2de1a75e8fbc65808051ff1983d19a/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Pagelet API

## 1. 프로젝트 개요

NestJS 기반 멀티테넌트 블로그/콘텐츠 플랫폼 백엔드 API (`{slug}.pagelet.kr` 서브도메인 구조)

---

## 2. 기술 스택

| 카테고리   | 기술                  | 버전             |
| ---------- | --------------------- | ---------------- |
| Framework  | NestJS                | ^11.0.1          |
| Language   | TypeScript            | ^5.7.3           |
| Database   | PostgreSQL (Supabase) | -                |
| ORM        | TypeORM               | ^0.3.28          |
| Auth       | JWT, Passport         | ^11.0.2, ^11.0.5 |
| Storage    | AWS S3 SDK            | ^3.971.0         |
| Cache      | Redis (ioredis)       | ^5.9.2           |
| Validation | class-validator, Joi  | ^0.14.1, ^18.0.2 |
| API Docs   | Swagger               | ^11.2.5          |
| Test       | Jest                  | ^30.0.0          |

---

## 3. 디렉토리 구조

```
src/
├── main.ts                    # 앱 진입점
├── app.module.ts              # 루트 모듈
├── config/                    # 설정 (DB, JWT, S3 등)
├── database/                  # 데이터소스, 마이그레이션
├── auth/                      # 인증 (JWT, OAuth, Guards)
│   ├── oauth/                 # Kakao, Naver OAuth
│   ├── guards/                # JwtAuth, AccountStatus, AdminSite
│
```

</details>
