---
name: Jerdirlson__Congreso-de-ingenierias-UPB-2026
source: https://github.com/Jerdirlson/Congreso-de-ingenierias-UPB-2026/blob/573be930bf28de5275a70018858d18d02a1378c8/CLAUDE.md
repo: Jerdirlson/Congreso-de-ingenierias-UPB-2026
kind: claude-md
stars: 0
last_pushed: 2026-06-13T16:30:41Z
license: unknown
score: 9
domains: [web-development, fullstack, laravel, vue]
tags: [production-guardrails, tech-stack, convention-driven]
curated: 2026-06-15
curated_by: config-scout
---

# Jerdirlson/Congreso-de-ingenierias-UPB-2026 — claude-md

**Why it's worth keeping:** The 'Production Warning' regarding database migrations is a vital safety pattern for AI agents, alongside an explicit 'Conventions' section to prevent CSS sprawl.

**Summary:** A highly structured project context file that includes critical production guardrails and specific environment setup instructions. It bridges the gap between code and intent by defining roles, conventions, and documentation paths.

**Source credibility:** Low social proof due to zero stars, but the highly specific technical detail suggests it is a real-world engineering project.

**Recency:** Extremely current; it uses cutting-edge versions like Laravel 12 and Tailwind v4.

**Source:** [Jerdirlson/Congreso-de-ingenierias-UPB-2026/CLAUDE.md](https://github.com/Jerdirlson/Congreso-de-ingenierias-UPB-2026/blob/573be930bf28de5275a70018858d18d02a1378c8/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Congreso Ingenierías 2026 — Contexto del proyecto

Plataforma del **II Congreso Internacional de Ingeniería 2026** (UPB Bucaramanga):
inscripciones, envío y revisión de ponencias, pagos, videoponencias y panel de administración.

> ⚠️ **App en producción.** Cambios de BD **solo por migraciones**; nada de breaking
> changes en la API. Trabajar directo en `main` está permitido, pero commitear/pushear
> solo cuando el usuario lo pida.

## Stack
- **Frontend** (`frontend/`): Vue 3 + TypeScript + Vite + Tailwind CSS v4 (`@tailwindcss/vite`, sin `tailwind.config.js`). Pinia para estado, Vue Router 4.
- **Backend** (`backend/`): PHP Laravel 12 + Sanctum (tokens) + Spatie Permission (roles) + Spatie Media Library.
- **Infra**: Docker Compose — MySQL 8, Redis 7, Nginx, Mailpit, phpMyAdmin, queue worker.
- PHP/Composer **solo dentro de Docker** (no hay PHP nativo en local ni en el servidor).

## Cómo correr
```bash
docker compose up --build
# Frontend http://localhost:5173 · API http://localhost:8000/api · phpMyAdmin http://localhost:8080
docker compose exec backend php artisan migrate --force   # en prod usar --force
docker compose exec backend php artisan tinker            # consola
```
```

</details>
