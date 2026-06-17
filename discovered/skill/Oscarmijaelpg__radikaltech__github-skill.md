---
name: Oscarmijaelpg__radikaltech__github-skill
source: https://github.com/Oscarmijaelpg/radikaltech/blob/26123de081e16dfd24024b82bbf2274a8e7d2c07/skills/github_skill.md
repo: Oscarmijaelpg/radikaltech
kind: skill
stars: 0
last_pushed: 2026-06-16T02:01:00Z
license: unknown
score: 9
domains: [devops, git-workflows, security, ci-cd]
tags: [deploy, github, safety, monorepo]
curated: 2026-06-16
curated_by: config-scout
---

# Oscarmijaelpg/radikaltech — skill

**Why it's worth keeping:** The specific regex patterns for secret scanning and the multi-stage verification process (inspection -> gate -> confirmation) are excellent templates for production agents.

**Summary:** A highly structured, safety-first deployment workflow that incorporates automated secret detection, typechecking/testing gates, and strict rebase policies.

**Source credibility:** Low social proof (0 stars), but demonstrates high technical depth in workflow automation.

**Recency:** Current; uses modern toolchains like pnpm and GitHub CLI.

**Source:** [Oscarmijaelpg/radikaltech/skills/github_skill.md](https://github.com/Oscarmijaelpg/radikaltech/blob/26123de081e16dfd24024b82bbf2274a8e7d2c07/skills/github_skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: deploy-github
description: Sube los commits locales a origin siguiendo las prácticas del repo (sync sin merge-commits, gates de calidad, detección de secretos, sin force-push). Invoca cuando el user diga "push", "subir cambios", "deploy a GitHub", "actualiza el repo", "sube esto".
---

# Deploy to GitHub — Radikal

Pusher seguro para trabajo en equipo. El objetivo es **evitar pushes rotos, mezclas de archivos entre devs, y filtrar secretos**.

## Flujo general

Ejecuta las fases en orden. Si alguna falla, detente y reporta — nunca sigas adelante con errores.

### Fase 1 — Inspección (paralelo)

Lanza estos comandos en una sola tool-call de Bash paralelas:

- `git rev-parse --abbrev-ref HEAD` → branch actual
- `git status --porcelain` → cambios no commiteados
- `git fetch origin --quiet` → refresca refs remotos
- `git log --oneline origin/HEAD..HEAD` → commits que faltan por pushear
- `git log --oneline HEAD..origin/HEAD` → commits que me faltan (behind)

Interpreta los resultados antes de continuar.

### Fase 2 — Estado del working tree

Si hay cambios no commiteados:

- Lista al user qué archivos cambiaron.
- **Pregunta** qué hacer:
  - (a) commitearlos ahora (usa el ski
```

</details>
