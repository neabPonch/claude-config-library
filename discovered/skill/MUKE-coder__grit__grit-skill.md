---
name: MUKE-coder__grit__grit-skill
source: https://github.com/MUKE-coder/grit/blob/625670779affeb0f5b48093ffeab0fed28e818f9/GRIT_SKILL.md
repo: MUKE-coder/grit
kind: skill
stars: 40
last_pushed: 2026-06-14T06:57:50Z
license: unknown
score: 8
domains: [full-stack, cli-tools, monorepo, go, nextjs]
tags: [framework-rules, project-onboarding, architecture-map]
curated: 2026-06-15
curated_by: config-scout
---

# MUKE-coder/grit — skill

**Why it's worth keeping:** It provides explicit command-line references and high-level structural mapping, which prevents AI from hallucinating file locations or manual sync steps in a complex monorepo.

**Summary:** Acts as a comprehensive 'mental model' guide that explains the framework's CLI-driven workflow, architecture, and cross-package type synchronization.

**Source credibility:** Low-to-moderate; 40 stars suggests it is a niche developer tool rather than an industry standard.

**Recency:** Very current; utilizes modern stacks like Next.js App Router and Wails.

**Source:** [MUKE-coder/grit/GRIT_SKILL.md](https://github.com/MUKE-coder/grit/blob/625670779affeb0f5b48093ffeab0fed28e818f9/GRIT_SKILL.md) · 40★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Grit Framework — LLM Skill Guide

> **This document teaches AI assistants (Claude, Cursor, Kilo Code, etc.) how to work with the Grit framework.** Read this file completely before writing any code in a Grit project.

---

## What is Grit?

Grit is a full-stack meta-framework that combines **Go** (backend) + **React/Next.js** (frontend) in a monorepo. It provides:

- A **CLI tool** (`grit`) that scaffolds entire projects and generates full-stack resources
- A **Go API** with Gin + GORM + PostgreSQL
- A **Next.js web app** with App Router + Tailwind + shadcn/ui
- A **Filament-like admin panel** with resource definitions, DataTables, forms, and widgets
- **Native desktop apps** with Wails (Go + React + SQLite) — `grit new-desktop`
- **Social login** out of the box — Google + GitHub OAuth2 via Gothic, with account linking
- **Batteries included**: file storage (S3), email (Resend), background jobs (asynq), cron, Redis caching, AI integration (Claude/OpenAI), security (Sentinel), observability (Pulse)
- **Auto-generated API docs** via gin-docs — zero-annotation OpenAPI spec with interactive UI
- A **shared package** with Zod schemas, TypeScript types, and constants

**Think of it as:*
```

</details>
