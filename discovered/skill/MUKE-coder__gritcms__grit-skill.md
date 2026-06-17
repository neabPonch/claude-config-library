---
name: MUKE-coder__gritcms__grit-skill
source: https://github.com/MUKE-coder/gritcms/blob/f799356ec9f7e564060a805abc977e26dd36d23f/GRIT_SKILL.md
repo: MUKE-coder/gritcms
kind: skill
stars: 17
last_pushed: 2026-04-06T00:18:46Z
license: unknown
score: 8
domains: [fullstack, cli-tools, monorepo]
tags: [go, react, scaffolding, framework-guide]
curated: 2026-06-14
curated_by: config-scout
---

# MUKE-coder/gritcms — skill

**Why it's worth keeping:** It explicitly documents the side effects of CLI commands (which files are created vs. modified), preventing agents from writing manual boilerplate when a scaffold tool exists.

**Summary:** A highly structured domain-specific guide that teaches an AI how to navigate a custom Go + Next.js monorepo using project-specific CLI tools.

**Source credibility:** Developing open-source project with recent, active maintenance.

**Recency:** Extremely current; reflects modern monorepo and agentic workflow requirements.

**Source:** [MUKE-coder/gritcms/GRIT_SKILL.md](https://github.com/MUKE-coder/gritcms/blob/f799356ec9f7e564060a805abc977e26dd36d23f/GRIT_SKILL.md) · 17★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Grit Framework — LLM Skill Guide

> **This document teaches AI assistants (Claude, Cursor, Kilo Code, etc.) how to work with the Grit framework.** Read this file completely before writing any code in a Grit project.

---

## What is Grit?

Grit is a full-stack meta-framework that combines **Go** (backend) + **React/Next.js** (frontend) in a monorepo. It provides:

- A **CLI tool** (`) that scaffolds entire projects and generates full-stack resources
- A **Go API** with Gin + GORM + PostgreSQL
- A **Next.js web app** with App Router + Tailwind + shadcn/ui
- A **Filament-like admin panel** with resource definitions, DataTables, forms, and widgets
- **Batteries included**: file storage (S3), email (Resend), background jobs (asynq), cron, Redis caching, AI integration (Claude/OpenAI), security (Sentinel), observability (Pulse)
- **Auto-generated API docs** via gin-docs — zero-annotation OpenAPI spec with interactive UI
- A **shared package** with Zod schemas, TypeScript types, and constants

**Think of it as:** Laravel + Filament, but with Go + React instead of PHP + Blade.

---

## Quick Reference — CLI Commands

`ash
# Create a new project
grit new myapp                    # Full m
```

</details>
