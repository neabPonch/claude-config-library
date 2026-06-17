---
name: semaj90__deeds_web_app__claude
source: https://github.com/semaj90/deeds_web_app/blob/858b77e217718030b0ad2e5fc874cf0e1ed94d3e/sveltekit-frontend/claude.md
repo: semaj90/deeds_web_app
kind: claude-md
stars: 0
last_pushed: 2026-06-15T21:22:47Z
license: unknown
score: 8
domains: [backend-api, ai-agents, data-architecture]
tags: [architectural-guardrails, rag, rabbitmq, xstate, streaming]
curated: 2026-06-16
curated_by: config-scout
---

# semaj90/deeds_web_app — claude-md

**Why it's worth keeping:** The 'Identity Contract' is a brilliant technique to prevent AI from making structural database errors. The file also includes ready-to-use code templates for complex patterns like background job processing and SSE streaming.

**Summary:** Establishes strict architectural guardrails (Frozen Identity Contract) alongside implementation patterns for RabbitMQ, RAG, and KAG. It provides both high-level business logic constraints and low-level technical templates.

**Source credibility:** Low star count, but the depth of technical detail suggests a sophisticated real-world enterprise application.

**Recency:** Extremely current; uses modern patterns relevant to today's AI agentic development workflows.

**Source:** [semaj90/deeds_web_app/sveltekit-frontend/claude.md](https://github.com/semaj90/deeds_web_app/blob/858b77e217718030b0ad2e5fc874cf0e1ed94d3e/sveltekit-frontend/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Tactical Error Fixing Guide - Phase 96 + Parent Atlas P0–P7

## ⚡ PRIORITY: Parent Atlas Frozen Identity Contract (June 14, 2026)

**Read first**: `../memory/parent-atlas-frozen-identity-contract.md`

This project now operates under the **Parent Atlas P0–P7 Roadmap**. All error fixing, packet retrieval, and GPU acceleration work must follow:

1. **Frozen Identity** — no feature_id-only joins, always source_ref + directory_path
2. **Postgres is Truth** — Qdrant/Redis/Neo4j are mirrors or cache only
3. **Strict Retrieval Order** — BitFrost → Postgres → Qdrant → Neo4j (k-hop bounded)
4. **Hard Fail Conditions** — no placeholder files, no silent fallbacks
5. **No Unbounded Traversal** — all graph queries must bound k-hops

See `Parent Atlas Frozen Identity Contract` section in root CLAUDE.md for P0–P7 roadmap + key commands.

---

## Current Diagnostics Regression Checkpoint

- Run `npm run test:diagnostics` from `sveltekit-frontend` after diagnostics-related changes.
- Unit-only slice: `npm run test:diagnostics:unit`
- Browser-only slice: `npm run test:diagnostics:e2e`
- VS Code task labels: `Diagnostics Regression Slice`, `Diagnostics Regression Slice (Unit)`, and `Diagnosti
```

</details>
