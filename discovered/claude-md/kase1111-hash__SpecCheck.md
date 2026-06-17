---
name: kase1111-hash__SpecCheck
source: https://github.com/kase1111-hash/SpecCheck/blob/81996f6c8fd5a32801d52b1f38aef9b8d3cc592c/claude.md
repo: kase1111-hash/SpecCheck
kind: claude-md
stars: 1
last_pushed: 2026-02-22T23:16:49Z
license: mit
score: 9
domains: [mobile, fullstack, monorepo]
tags: [react-native, architecture-first, typescript]
curated: 2026-06-14
curated_by: config-scout
---

# kase1111-hash/SpecCheck — claude-md

**Why it's worth keeping:** Provides explicit 'Key Patterns' for file naming and module exports, alongside a detailed architectural pipeline that is essential for AI reasoning over complex features.

**Summary:** A highly structured technical overview of a mobile monorepo detailing stack, folder hierarchy, and core processing logic.

**Source credibility:** Low star count but the high level of technical specificity suggests an authentic, well-engineered project.

**Recency:** Very current; uses modern Expo 52 and React Native standards.

**Source:** [kase1111-hash/SpecCheck/claude.md](https://github.com/kase1111-hash/SpecCheck/blob/81996f6c8fd5a32801d52b1f38aef9b8d3cc592c/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SpecCheck

X-ray vision for tech claims. A mobile app that identifies electronic components via camera and calculates physical limits to verify seller specifications.

## Tech Stack

- **Mobile**: React Native 0.76 + Expo 52, TypeScript, Zustand, SQLite, TensorFlow.js
- **Backend**: Hono on Cloudflare Workers, Supabase (PostgreSQL), Claude API
- **Monorepo**: npm workspaces with shared types package

## Project Structure

```
apps/
  mobile/src/          # 69 TypeScript files, feature-organized
    analysis/          # Claim validation & constraint chains
    ar/                # AR overlay & component markers
    camera/            # Camera capture & frame handling
    recognition/       # ML detection & OCR
    pipeline/          # Processing orchestration
    database/          # SQLite repositories
    datasheet/         # Spec retrieval & caching
    store/             # Zustand state
    ui/                # Screens & components
  backend/src/         # 16 TypeScript files
    routes/            # API endpoints (datasheet, analyze, community)
    services/          # DatasheetService, LLMService
    db/                # Database queries
packages/
  shared-types/        # Ty
```

</details>
