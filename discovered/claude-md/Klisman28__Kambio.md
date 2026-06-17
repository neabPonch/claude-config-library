---
name: Klisman28__Kambio
source: https://github.com/Klisman28/Kambio/blob/c53f28368c7c4a99f590602f654cf989d7b7a5d1/CLAUDE.md
repo: Klisman28/Kambio
kind: claude-md
stars: 0
last_pushed: 2026-05-21T23:25:00Z
license: unknown
score: 8
domains: [backend-api, web-frontend, financial-software]
tags: [fastapi, vue3, architecture-patterns, domain-logic]
curated: 2026-06-16
curated_by: config-scout
---

# Klisman28/Kambio — claude-md

**Why it's worth keeping:** Features high-value techniques like 'read-order' sequencing, mission-critical financial integrity rules (calculating vs. storing balances), and a mandatory task-wrapup output format.

**Summary:** Defines strict architectural patterns and domain-specific logic for a financial full-stack application using FastAPI and Vue 3.

**Source credibility:** Low; appears to be a small or private repository with minimal social proof.

**Recency:** Current; aligns well with modern full-stack development workflows and Claude Code's capabilities.

**Source:** [Klisman28/Kambio/CLAUDE.md](https://github.com/Klisman28/Kambio/blob/c53f28368c7c4a99f590602f654cf989d7b7a5d1/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Lee primero:
- AGENTS.md
- docs/PRD.md
- docs/ARCHITECTURE.md
- docs/TASKS.md

## Rol esperado
Actúa como arquitecto de software senior y desarrollador backend/frontend senior.

## Objetivo
Construir Finances con:
- backend FastAPI
- frontend Vue 3 + TypeScript
- MySQL
- tema comprado como base visual

## Reglas backend
- Usar FastAPI
- Versionar API desde el inicio: `/api/v1`
- Separar:
  - ORM models
  - Pydantic schemas
  - services
  - repositories
- Usar SQLAlchemy + Alembic
- Usar transacciones ACID para operaciones financieras
- Nunca persistir saldo editable de cliente
- Calcular saldo desde historial de transacciones

## Reglas frontend
- Usar Vue 3 + TypeScript + Vite
- Usar Pinia y Vue Router
- Mantener el tema en `frontend/src/theme`
- Crear lógica del sistema en `frontend/src/modules`
- No mezclar código demo del tema con la lógica del negocio
- No rehacer estilos base del tema sin necesidad

## Reglas de calidad
- Primero plan, luego cambios
- Mostrar archivos a tocar antes de cambios grandes
- Preferir cambios incrementales
- Al final de cada tarea, responder con:
  - resumen
  - archivos cambiados
  - riesgos
  - siguiente paso recomendado

## Módulos V
```

</details>
