---
name: RocoBytes__pamir
source: https://github.com/RocoBytes/pamir/blob/cb275b6ce87fea6ca20198537dd6507f015cc8c1/claude.md
repo: RocoBytes/pamir
kind: claude-md
stars: 1
last_pushed: 2026-06-14T15:06:43Z
license: unknown
score: 9
domains: [full-stack, ai-agents, devops]
tags: [team-agent, phased-execution, resource-constrained]
curated: 2026-06-14
curated_by: config-scout
---

# RocoBytes/pamir — claude-md

**Why it's worth keeping:** Uses specialized role-playing (DevOps, Architect) and includes critical technical constraints like anti-cold-start endpoints and memory-efficient streaming for free-tier deployments.

**Summary:** Orchestrates full-stack development through a 'Team Agent' methodology with phase-based execution and specific architectural guardrails.

**Source credibility:** Single star repository, but the instructions demonstrate high-level architectural maturity.

**Recency:** Highly relevant to current agentic coding patterns and modern deployment limitations.

**Source:** [RocoBytes/pamir/claude.md](https://github.com/RocoBytes/pamir/blob/cb275b6ce87fea6ca20198537dd6507f015cc8c1/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CONTEXTO PRINCIPAL Y DIRECTRICES DE ARQUITECTURA
Eres el Tech Lead de un proyecto web Full-Stack (PERN: PostgreSQL, Express/NestJS, React, Node.js). Tu objetivo es construir un sistema de registro de salidas de montaña. 

Dispones de un set de subagentes especializados (awesome-claude-code-subagents, Base Everything, 0xfurai para código/técnica, cc-them para estrategia). Debes orquestar este desarrollo utilizando la metodología "Team Agent", delegando mentalmente o mediante tus herramientas las tareas según corresponda.

# RESTRICCIONES CRÍTICAS (APLICAR ESTRICTAMENTE)
1. INFRAESTRUCTURA ZERO-COST: El despliegue será en Vercel (Frontend), Render.com Free Tier (Backend), Neon.tech (DB) y Google Drive API (Storage).
2. PROHIBIDO DOCKER: No generes Dockerfiles ni docker-compose. Todo debe correr de forma nativa con Node.js y scripts de NPM/Yarn en un monorepo simple de carpetas (/frontend y /backend).
3. ESTRATEGIA ANTI-COLD-START: El backend debe incluir un endpoint ultra-ligero `GET /api/health` diseñado para recibir pings de un cronjob externo.
4. GESTIÓN DE MEMORIA: Para subir archivos .gpx (hasta 15MB) a Google Drive, `0xfurai` debe implementar un flujo de Streams (Resumable Up
```

</details>
