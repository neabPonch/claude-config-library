---
name: paniklas__spotteq-eshop
source: https://github.com/paniklas/spotteq-eshop/blob/b152ade5f21a7948668ed0d5ad2509a8a62ee72e/CLAUDE.md
repo: paniklas/spotteq-eshop
kind: claude-md
stars: 0
last_pushed: 2026-06-07T15:04:23Z
license: unknown
score: 9
domains: [fullstack, web-development]
tags: [context-switching, guardrails, production-ready]
curated: 2026-06-15
curated_by: config-scout
---

# paniklas/spotteq-eshop — claude-md

**Why it's worth keeping:** It utilizes distinct execution modes (Discuss, Implement, Review) to control AI behavior and includes a highly detailed 'Active Projects' section for seamless context switching between different tech stacks.

**Summary:** A high-context multi-project configuration that defines environment specs and strict behavioral guardrails for various client workloads.

**Source credibility:** High; reflects real-world production environments across multiple active projects.

**Recency:** Very current, referencing modern versions like Node 22 and Tailwind v4.

**Source:** [paniklas/spotteq-eshop/CLAUDE.md](https://github.com/paniklas/spotteq-eshop/blob/b152ade5f21a7948668ed0d5ad2509a8a62ee72e/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

# Core Behavior

- Follow explicit user instructions first.
- Preserve existing architecture, conventions, and project structure.
- Minimize scope of changes.
- Prefer simple, maintainable implementations.
- Avoid assumptions.
- State uncertainty clearly when confidence is low.

---

# Instruction Priority

When instructions conflict, follow this order:

1. Explicit user instructions
2. Safety and irreversible action constraints
3. Preserve existing work and architecture
4. Minimize scope of changes
5. Simplicity and maintainability
6. Performance and optimization

---

# Environment

## Node Environment

- Node.js 22
- pnpm preferred
- Next.js App Router
- Turbopack enabled when applicable

## Python Environment

- Python 3.12
- venv or uv depending on project
- Django projects typically use DRF
- Celery + Redis for async/background jobs

## Database

- PostgreSQL primary database
- Prisma ORM for Next.js projects
- Django ORM for backend services
- Supabase used in selected projects

## Infrastructure

- Ubuntu VPS
- Nginx
- Gunicorn
- systemd
- DigitalOcean
- Cloudflare
- Vercel

## Frontend Conventions

- Tailwind CSS
- shadcn/ui
- React Hook Form
- Server Actions
```

</details>
