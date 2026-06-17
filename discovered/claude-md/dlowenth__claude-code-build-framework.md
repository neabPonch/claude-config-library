---
name: dlowenth__claude-code-build-framework
source: https://github.com/dlowenth/claude-code-build-framework/blob/eb91e2a30abff0471001446940585c1659df4c10/claude.md
repo: dlowenth/claude-code-build-framework
kind: claude-md
stars: 8
last_pushed: 2026-04-14T12:33:36Z
license: mit
score: 9
domains: [software-architecture, fullstack-development, security]
tags: [governance, phase-gates, deterministic-execution]
curated: 2026-06-15
curated_by: config-scout
---

# dlowenth/claude-code-build-framework — claude-md

**Why it's worth keeping:** The 'Phase Gate Rule' is a brilliant technical workaround for context compaction, and the 'Deterministic vs Probabilistic' principle optimizes for reliability by forcing script use over LLM reasoning.

**Summary:** A high-rigor governance framework that treats Claude Code as a professional engineer following a strict build contract rather than just a coding assistant.

**Source credibility:** High; comes from a specialized governance framework repository with recent maintenance.

**Recency:** Very current; demonstrates deep understanding of Claude Code's specific behavior regarding context management.

**Source:** [dlowenth/claude-code-build-framework/claude.md](https://github.com/dlowenth/claude-code-build-framework/blob/eb91e2a30abff0471001446940585c1659df4c10/claude.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude.md

## Purpose
This document defines the mandatory architectural, security, and execution framework for all new application builds using Claude Code.

It is not a PRD.
It is the governing build contract.

Every new project must comply unless explicitly overridden in writing.

---

# 0. Project Metadata Template (Required at Kickoff)

Every new project must declare the following before any planning begins. The PRD fills in these values; this section defines the required fields.

| Field | Value |
|---|---|
| Project Name | `<<APP_NAME>>` |
| Owner | `<<OWNER>>` |
| Date | `<<DATE>>` |
| Version | `<<VERSION>>` |
| Status | Draft / In Review / Approved |
| Expected User Scale | `<<SCALE>>` |
| Tenancy Model | Single-tenant / Multi-tenant (shared schema) / Multi-tenant (isolated) |
| Auth Provider | Discord OAuth (default) / Clerk / Other |
| Billing Provider | None / Clerk Billing / Stripe / Other |
| Backend | Supabase (default) |
| Frontend Framework | React (default) / Other |
| Deployment Target | Railway (default) / Other |
| Edge Functions | Supabase Edge Functions (default) / Other |
| External Integrations | `<<LIST>>` |
| Observability | None / PostHog / Sentry / Ot
```

</details>
