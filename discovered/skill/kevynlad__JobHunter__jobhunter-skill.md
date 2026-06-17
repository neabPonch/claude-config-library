---
name: kevynlad__JobHunter__jobhunter-skill
source: https://github.com/kevynlad/JobHunter/blob/191ddeb0de4f1afcf5a521e3708a3709306effbe/JOBHUNTER_SKILL.md
repo: kevynlad/JobHunter
kind: skill
stars: 0
last_pushed: 2026-05-19T21:53:55Z
license: unknown
score: 8
domains: [backend-api, agents-ai, security, serverless]
tags: [architecture-guide, multi-tenant, byok, serverless-patterns]
curated: 2026-06-16
curated_by: config-scout
---

# kevynlad/JobHunter — skill

**Why it's worth keeping:** It outlines critical failure modes like serverless timeouts, database connection pooling in worker threads, and a robust BYOK security pattern.

**Summary:** Defines architectural boundaries between ephemeral webhooks (Vercel) and long-running background workers (GitHub Actions).

**Source credibility:** Low public reputation (0 stars), but demonstrates sophisticated engineering thought regarding distributed systems.

**Recency:** Current; addresses modern serverless-to-LLM orchestration challenges.

**Source:** [kevynlad/JobHunter/JOBHUNTER_SKILL.md](https://github.com/kevynlad/JobHunter/blob/191ddeb0de4f1afcf5a521e3708a3709306effbe/JOBHUNTER_SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: jobhunter-architect
description: Diretrizes de arquitetura, segurança e limites para o projeto JobHunter (Multi-Tenant Serverless). Consute sempre esta skill ao implementar novas features.
risk: high
source: local
date_added: '2026-03-30'
---

# 🎯 JobHunter Multi-Tenant - Native Skill & Architecture Guide

Você é um Arquiteto de Software Sênior especializado em sistemas Serverless, Python Assíncrono e Integrações de LLMs (Gemini). Use esta skill sempre que trabalhar na base de código do **JobHunter** para garantir que as restrições de infraestrutura, segurança (BYOK), e orquestração sejam respeitadas.

## 🏗️ 1. Arquitetura do Sistema (Visão Geral)

O JobHunter passou de um script local síncrono para uma arquitetura descentralizada, dividida em dois grandes blocos:

### A. Vercel (Bot / Webhooks) - "O Atendente Rápido"
- **Função:** Receber os comandos do Telegram (`/start`, `/set_key`, `/set_profile`, botões).
- **Regra de Ouro:** A Vercel **MATA** qualquer requisição que dure mais do que 10 a 60 segundos (dependendo do plano).
- **Proibido:** NUNCA execute scraping (`jobspy`) ou chamadas pesadas do LLM (`gemini`) dentro do escopo da chamada da Vercel.
- **Padrão:** Receb
```

</details>
