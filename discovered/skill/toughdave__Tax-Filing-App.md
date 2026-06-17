---
name: toughdave__Tax-Filing-App
source: https://github.com/toughdave/Tax-Filing-App/blob/fa756a1bfc8e08ab5ee5f3c498bb71990064564b/skill.md
repo: toughdave/Tax-Filing-App
kind: skill
stars: 0
last_pushed: 2026-03-23T21:59:36Z
license: unknown
score: 7
domains: [fintech, security]
tags: [guardrails, escalation-logic, domain-constraints]
curated: 2026-06-16
curated_by: config-scout
---

# toughdave/Tax-Filing-App — skill

**Why it's worth keeping:** The 'Escalation Triggers' section provides a high-level pattern for defining exactly which actions require human approval in sensitive workflows. The 'Scope Boundaries' also serve as excellent guardrails to prevent LLM hallucinations from expanding project scope.

**Summary:** Defines domain-specific capabilities, security standards, and strict operational boundaries for a tax filing agent. It explicitly dictates when an agent must stop autonomy and seek human intervention.

**Source credibility:** Low credibility; single developer with no community traction or social proof.

**Recency:** 

**Source:** [toughdave/Tax-Filing-App/skill.md](https://github.com/toughdave/Tax-Filing-App/blob/fa756a1bfc8e08ab5ee5f3c498bb71990064564b/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# skill.md

## Capability Matrix

### Product UX
- Guided multi-path filing interview (individual, self-employed, company)
- Progressive disclosure to reduce user overwhelm
- Bilingual UI for core workflows (EN/FR)

### Identity & Security
- OAuth-ready account model
- Database-backed sessions
- Security headers and audit event logging
- Baseline secure coding controls documented and enforceable

### Tax Workflow Engine
- Filing-year aware return records
- Required-field gating and draft/review state progression
- Prior-year carry-forward for continuity
- Submission preparation interface with provider abstraction

### Platform
- Next.js fullstack architecture
- Prisma + PostgreSQL domain model
- API routes for authenticated filing operations
- CI/CD pipeline scaffolding with quality gates

## Quality Standards

- Strict TypeScript compilation
- Passing lint, tests, and production build before release
- No sensitive data in logs or source control
- Deterministic status transitions

## Scope Boundaries (Current)

- Canada-only implementation scope
- Sandbox submission provider for preparation stage
- Production e-filing/certification work remains roadmap item

## Escalation Triggers
```

</details>
