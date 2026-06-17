---
name: crowi__crowi__skill
source: https://github.com/crowi/crowi/blob/4b5f6d043fae61e77535fd9a0456448d9381452e/.claude/skills/crowi-migration/SKILL.md
repo: crowi/crowi
kind: skill
stars: 1099
last_pushed: 2026-06-14T15:59:26Z
license: mit
score: 9
domains: [architectural-migration, agents-ai, workflow-orchestration]
tags: [migration, state-management, role-based]
curated: 2026-06-15
curated_by: config-scout
---

# crowi/crowi — skill

**Why it's worth keeping:** The role-based workflow (planner → implementer → reviewer) and the structured `.migration-state` JSON pattern provide a highly robust framework for large-scale refactors. Including explicit 'old vs new' code patterns acts as an in-context template to ensure high-fidelity migrations.

**Summary:** Orchestrates a complex architectural migration from Express/Swig to Hono/Next.js using specialized agent roles. It utilizes an externalized state management system to track long-running tasks across multiple sessions.

**Source credibility:** High; derived from an active, well-maintained open-source project (1k+ stars).

**Recency:** 

**Source:** [crowi/crowi/.claude/skills/crowi-migration/SKILL.md](https://github.com/crowi/crowi/blob/4b5f6d043fae61e77535fd9a0456448d9381452e/.claude/skills/crowi-migration/SKILL.md) · 1099★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: crowi-migration
description: |
  Crowi 2.0 移行ワークフロー。Express/Swig から Next.js + Hono への移行時に自動適用。
  キーワード: migrate, 移行, Express, Swig, legacy, 旧実装
globs:
  - "packages/api/src/hono/**"
  - "packages/api-contract/src/**"
  - "packages/web/src/app/**"
---

# Crowi 2.0 Migration Skill

Crowi の旧 Express + Swig + jQuery を、新 Hono API + Next.js に段階的に置き換える。
1人開発・main 直コミット運用が前提。

> 注: 旧 Express/Swig レイヤーと中間の ts-rest 実装は RFC-0006 (2026-05-22 main マージ)
> で完全撤去済み。core wiki 機能の移行はほぼ完了しており、この skill は主に残作業・
> 新規エンドポイント追加の参照用。

## 実態のアーキテクチャ

```
crowi/                            # Turborepo + pnpm workspace
├── apps/crowi-site/              # crowi.wiki LP + docs (移行対象外)
├── crowi.config.json             # dev runner config (plugins + active drivers)
├── .env(.example)                # dev runtime env (repo root で読まれる)
└── packages/
    ├── api/                      # Hono API (port 4301)
    │   └── src/
    │       ├── hono/             # ★ Hono app: handlers/ (admin/ 含む) + middleware/ + app.ts
    │       ├── models/           # Mongoose
    │       ├── crowi/            # boot sequence
    │       └── util/             # helpers
    ├── api-contract/             # Hono (@hono/zod-open
```

</details>
