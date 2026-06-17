---
name: kjahir__wealth360__project-claude
source: https://github.com/kjahir/wealth360/blob/ff262af2ea98e266f35cbf1e5191850a619de0f5/docs/ai/project-claude.md
repo: kjahir/wealth360
kind: claude-md
stars: 0
last_pushed: 2026-06-16T03:10:51Z
license: mit
score: 9
domains: [backend-api, microservices, infrastructure]
tags: [system-architecture, microservices, technical-context]
curated: 2026-06-16
curated_by: config-scout
---

# kjahir/wealth360 — claude-md

**Why it's worth keeping:** The 'Non-Negotiable Constraints' section is vital for preventing common AI errors, while the navigation/port tables provide immediate structural awareness for an agent.

**Summary:** A high-density technical reference for a complex microservice architecture that defines global standards and service mappings.

**Source credibility:** Low social proof (0 stars) but shows evidence of highly intentional, manually curated documentation for a test ecosystem.

**Recency:** Highly current, using modern versions like Java 21 and Spring Boot 3.2.

**Source:** [kjahir/wealth360/docs/ai/project-claude.md](https://github.com/kjahir/wealth360/blob/ff262af2ea98e266f35cbf1e5191850a619de0f5/docs/ai/project-claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Wealth360 — Project-Level Claude Context (project-claude.md)

> This file provides the top-level project context. Read it once at the start of any Wealth360 session.
> For module-specific context, see the relevant `module-claude.md` in each service directory.

## Project Purpose

**Wealth360 is a Seyali Platform test ecosystem**, not a production banking application. Every design decision is optimized to exercise Seyali capabilities:

- Enterprise Discovery (service labels, actuators, OpenAPI endpoints)
- Enterprise Object Modeling (EOM JSON)
- Schema Ingestion (REST/GraphQL/gRPC/Avro/SQL/MongoDB schemas)
- Domain Tool Generation (domain-tools.json)
- Skill Framework (skills.json)
- Agent Orchestration (agents.json)
- Workflow Automation (workflows.json)
- Knowledge Graph Construction (knowledge-graph-model.json)
- Environment Drift Detection (intentional DEV/UAT/PROD divergence)

## Technology Stack Quick Reference

| Layer | Technology | Notes |
|---|---|---|
| Java Services | Spring Boot 3.2.5, Java 21, Maven | customer, portfolio, risk, compliance, relationship, product |
| Python Services | FastAPI, Python 3.12, UV | document-analysis, ai-advisor |
| JBoss Service | WildFly
```

</details>
