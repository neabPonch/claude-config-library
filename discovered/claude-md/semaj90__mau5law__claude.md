---
name: semaj90__mau5law__claude
source: https://github.com/semaj90/mau5law/blob/5eedd171a501c927400576c240d39fa8148dcbc2/sveltekit-frontend/claude.md
repo: semaj90/mau5law
kind: claude-md
stars: 1
last_pushed: 2026-04-24T05:23:29Z
license: unknown
score: 8
domains: [backend-api, agents-ai, data-engineering]
tags: [rabbitmq, rag, streaming, xstate, architectural-patterns]
curated: 2026-06-16
curated_by: config-scout
---

# semaj90/mau5law — claude-md

**Why it's worth keeping:** It provides concrete code blueprints for complex operations like RabbitMQ message durability, RAG/KAG logic, and SSE streaming, which prevents the AI from hallucinating generic implementations.

**Summary:** A high-density tactical guide combining project-specific diagnostic commands with deep architectural implementation patterns.

**Source credibility:** Low star count, but shows high-level engineering proficiency in distributed systems and AI patterns.

**Recency:** Extremely current; utilizes cutting-edge technologies like XState v5 and modern LLM/Vector DB integration patterns.

**Source:** [semaj90/mau5law/sveltekit-frontend/claude.md](https://github.com/semaj90/mau5law/blob/5eedd171a501c927400576c240d39fa8148dcbc2/sveltekit-frontend/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Tactical Error Fixing Guide - Phase 96

## Current Diagnostics Regression Checkpoint

- Run `npm run test:diagnostics` from `sveltekit-frontend` after diagnostics-related changes.
- Unit-only slice: `npm run test:diagnostics:unit`
- Browser-only slice: `npm run test:diagnostics:e2e`
- VS Code task labels: `Diagnostics Regression Slice`, `Diagnostics Regression Slice (Unit)`, and `Diagnostics Regression Slice (E2E)`.
- Coverage includes evidence diagnostics rendering, `/api/evidence/[id]` metadata normalization and `404` handling, `/api/rag/search` diagnostics payloads, and the focused evidence upload Playwright flow.

## Current Situation (2026-01-11 21:00 PST)

**Status:** RabbitMQ Integration + RAG/KAG/DAG Knowledge Base Updates
**XState v5 Migration:** Case machines rebuilt, idle-detection needs cleanup
**Focus:** Streaming/Chunking response optimization

---

## 🐰 RabbitMQ Background Job Architecture

### Why We Need It
JavaScript is single-threaded → Can't handle heavy tasks (AI analysis, OCR, case clustering) during HTTP requests → Queue jobs via RabbitMQ → Workers process asynchronously

### Integration Pattern

**Producer (Frontend → RabbitMQ):**
```typescript
// i
```

</details>
