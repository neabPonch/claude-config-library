---
name: davixedes__ZenithHarvest-API
source: https://github.com/davixedes/ZenithHarvest-API/blob/5e1d3957c11e37878ad75ae4293eac71ae2e2a2f/CLAUDE.md
repo: davixedes/ZenithHarvest-API
kind: claude-md
stars: 0
last_pushed: 2026-06-12T03:14:05Z
license: unknown
score: 9
domains: [backend-api, microservices, database-design]
tags: [java, spring-boot, postgresql, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# davixedes/ZenithHarvest-API — claude-md

**Why it's worth keeping:** Contains highly actionable technical constraints such as the 'NOT NULL' philosophy and precise SQL quoting requirements that prevent common AI generation errors.

**Summary:** Provides deep architectural context for a Java-based microservices monorepo, including specific database schema rules and service communication protocols.

**Source credibility:** Highly structured documentation from a specialized agricultural insurance project.

**Recency:** Very current, utilizing modern stacks like Java 21 and Spring Boot 3.5.

**Source:** [davixedes/ZenithHarvest-API/CLAUDE.md](https://github.com/davixedes/ZenithHarvest-API/blob/5e1d3957c11e37878ad75ae4293eac71ae2e2a2f/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Zenith Harvest

> Seguro paramétrico agrícola via satélite. Monitora lavouras por NDVI (Sentinel-2),
> detecta perdas com visão computacional + IA, e paga sinistros via PIX em até 48h.
> SaaS B2B para seguradoras. Projeto da Global Solution 2026/1 — FIAP (grupo Zenith).

Este arquivo orienta assistentes de IA (Claude Code etc.) a trabalhar neste repositório.
Leia antes de gerar ou alterar código.

---

## Visão geral

Zenith Harvest é um **monorepo de microsserviços Java (Spring Boot)**. O produto resolve a
dor do produtor rural que espera meses por um sinistro agrícola: satélite vê a lavoura,
IA decide, PIX cai. Vende-se para seguradoras (Brasilseg, Porto, Mapfre, Tokio Marine).

**Stack principal:** Java 21 + Spring Boot 3.5.14 + PostgreSQL + MongoDB + RabbitMQ + Spring AI (Ollama).

---

## Arquitetura — 3 serviços Java

| Serviço | Porta | Responsabilidade |
|---|---|---|
| `gateway` | 8080 | Borda. Roteamento, validação de JWT, rate limit. Spring Cloud Gateway (reativo/WebFlux). |
| `core-svc` | 8081 | Coração. CRUD de todo o domínio + auth/JWT + financeiro. Publica eventos no RabbitMQ. |
| `analise-svc` | 8082 | Visão computacional (NDVI/satélite) + IA generativa (Spring AI
```

</details>
