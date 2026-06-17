---
name: pankildesai1988__Generative-AI-Demos__project-context-claude
source: https://github.com/pankildesai1988/Generative-AI-Demos/blob/9403c68a8eb087bcd8acfbc66723557b01716ea2/ArNir/docs/Project-Context-Claude.md
repo: pankildesai1988/Generative-AI-Demos
kind: claude-md
stars: 0
last_pushed: 2026-06-12T08:01:23Z
license: unknown
score: 9
domains: [backend-api, ai-agents, enterprise-architecture]
tags: [.net, rag, architecture-guardrails]
curated: 2026-06-16
curated_by: config-scout
---

# pankildesai1988/Generative-AI-Demos — claude-md

**Why it's worth keeping:** The 'CRITICAL Architecture Rules' section provides essential guardrails against circular dependencies; mapping specific project responsibilities ensures the LLM respects strict boundary constraints during refactoring.

**Summary:** Provides an exhaustive architectural map of a multi-project .NET enterprise AI platform, detailing RAG pipelines, database schemas, and service boundaries.

**Source credibility:** Low-visibility personal repository, but contains extremely high information density for a developer guide.

**Recency:** Very current, referencing .NET 9 and modern enterprise AI patterns.

**Source:** [pankildesai1988/Generative-AI-Demos/ArNir/docs/Project-Context-Claude.md](https://github.com/pankildesai1988/Generative-AI-Demos/blob/9403c68a8eb087bcd8acfbc66723557b01716ea2/ArNir/docs/Project-Context-Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ArNir Enterprise AI Platform — Claude Project Context

## Platform Overview
ArNir is a production-grade **.NET 9** Enterprise AI Platform with 14 projects, 19 Admin controllers (MVC + Bootstrap 5), 12 API controllers (REST + Swagger), and 72 passing unit tests across 8 sprints.

## Core Capabilities
- **RAG Pipeline**: 4-step ingestion (Parse → Chunk → Embed → Store) for PDF/DOCX/TXT. Dual storage: SQL Server (relational) + PostgreSQL/pgvector (vectors). Background IngestionQueue + IngestionWorker.
- **Multi-Provider LLM**: OpenAI GPT-4, Google Gemini, Anthropic Claude — switchable at runtime via PlatformSettings DB table.
- **Prompt Engineering**: 3-layer resolution (DB → Config → Code). 5 styles: zero-shot, few-shot, role, rag, hybrid. Full version management: edit-creates-version, history timeline, rollback, side-by-side compare with JS diff.
- **Evaluation Layer (LLM-as-Judge)**: Auto-scores every RAG response on Relevance (0-1) and Faithfulness (0-1) using gpt-4o-mini. Persisted in EvaluationResults table. Dashboard with KPI cards, Chart.js trends, color-coded DataTable.
- **Agent Execution**: IPlannerAgent multi-step orchestration with AgentRunLog persistence.
- **Semantic
```

</details>
