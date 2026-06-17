---
name: CidQueiroz__PapoDados
source: https://github.com/CidQueiroz/PapoDados/blob/67730e4e068476d09e59ede1edf375929cfe2519/claude.md
repo: CidQueiroz/PapoDados
kind: claude-md
stars: 0
last_pushed: 2026-04-19T10:31:36Z
license: mit
score: 9
domains: [backend-api, web-frontend, agents-ai, saas-architecture]
tags: [fullstack, rag, data-viz, architectural-blueprint]
curated: 2026-06-16
curated_by: config-scout
---

# CidQueiroz/PapoDados — claude-md

**Why it's worth keeping:** The document excels at defining the exact API response contracts (JSON structures) and provides specific behavioral guidelines for the AI regarding security, error handling, and performance constraints.

**Summary:** A high-fidelity architectural blueprint that bridges business vision with strict technical implementation requirements.

**Source credibility:** Low social proof on GitHub, but indicates high-level professional engineering/architectural planning.

**Recency:** Very current; utilizes modern tech like Django 5.x, Vite, and OCI GenAI patterns.

**Source:** [CidQueiroz/PapoDados/claude.md](https://github.com/CidQueiroz/PapoDados/blob/67730e4e068476d09e59ede1edf375929cfe2519/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# PROJETO: PapoDados (SaaS)
**Versão:** 1.0 (MVP "Unicórnio")
**Autor:** Cidirclay Queiroz (Arquiteto de Soluções & Engenheiro de IA)
**Stack:** OCI Native | Django (Backend) | React (Frontend) | RAG Architecture

---

## 1. VISÃO GERAL E INTENÇÃO DO PRODUTO
O **PapoDados** é um SaaS B2B focado em democratizar a Business Intelligence (BI) para o mercado brasileiro (PMEs).
**A Promessa:** "Converse com seus dados". O usuário faz upload de planilhas (CSV/XLSX) e interage via chat em linguagem natural para obter insights, gráficos e relatórios, sem precisar saber SQL, Excel avançado ou Power BI.

**Diferencial Competitivo:**
1.  **Proatividade:** O sistema não espera perguntas; ele sugere insights ("Cards de Inteligência") assim que o upload é feito.
2.  **Agnóstico:** Aceita qualquer estrutura de dados tabular.
3.  **Segurança:** Execução blindada em ambiente Oracle Cloud (OCI).

---

## 2. ARQUITETURA TÉCNICA (HARD CONSTRAINTS)

### Infraestrutura (OCI - Oracle Cloud Infrastructure)
* **Compute:** VM Standard A1.Flex (ARM) hospedando o Docker/Podman.
* **Database:** Oracle Autonomous Database (ADW) para dados estruturados e vetoriais (Oracle AI Vector Search).
* **Storage:** OCI Obj
```

</details>
