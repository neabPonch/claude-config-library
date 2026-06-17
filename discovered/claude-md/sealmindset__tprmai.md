---
name: sealmindset__tprmai
source: https://github.com/sealmindset/tprmai/blob/b4a010e716f912ad5aadf37b4e271126f865cf66/CLAUDE.MD
repo: sealmindset/tprmai
kind: claude-md
stars: 0
last_pushed: 2026-04-02T21:13:14Z
license: unknown
score: 8
domains: [agents-ai, backend-api, security]
tags: [enterprise-grc, api-integration, ai-agents]
curated: 2026-06-15
curated_by: config-scout
---

# sealmindset/tprmai — claude-md

**Why it's worth keeping:** It includes essential 'API Integration Best Practices' (rate limiting/polling logic) that prevent an LLM from making destructive or inefficient API calls.

**Summary:** A highly structured technical brief that provides architectural context and critical operational constraints for an AI-driven GRC platform.

**Source credibility:** Low social proof (0 stars), but content demonstrates high-complexity enterprise architecture and specific tool integrations.

**Recency:** Very current; uses modern stacks like Azure AI Foundry, Next.js 16, and NeMo Guardrails.

**Source:** [sealmindset/tprmai/CLAUDE.MD](https://github.com/sealmindset/tprmai/blob/b4a010e716f912ad5aadf37b4e271126f865cf66/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AI TPRM Machine

An AI-powered Third Party Risk Management (TPRM) platform for automating vendor risk assessments, compliance monitoring, and audit workflows.

## Project Overview

This project integrates AI capabilities with enterprise GRC (Governance, Risk, and Compliance) platforms to streamline TPRM operations:

- **Vendor Risk Assessments**: Automated risk scoring and assessment workflows
- **Audit Management**: Integration with AuditBoard for OpsAudits operations
- **Compliance Monitoring**: Continuous monitoring of third-party vendors
- **Evidence Collection**: Automated evidence gathering and documentation

## Technology Stack

- **Runtime**: Node.js v22.12.0
- **Framework**: Next.js 16
- **AI Provider**: Claude via Azure AI Foundry (PRIMARY)
  - Primary: Claude Opus 4.6
  - Fallback: Claude Opus 4.5
  - OpenAI is optional alternative only
- **ORM**: Prisma with PostgreSQL
- **Auth**: OIDC + stateless JWT, database-driven RBAC (4 system roles)
- **UI**: Radix UI + Tailwind CSS
- **AI Safety**: Input sanitization, output validation, rate limiting, PII masking, NeMo Guardrails
- **Infra**: Docker Compose (app + PostgreSQL + mock-oidc), Terraform (Azure)
- **API Integrations
```

</details>
