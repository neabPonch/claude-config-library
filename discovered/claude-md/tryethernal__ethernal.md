---
name: tryethernal__ethernal
source: https://github.com/tryethernal/ethernal/blob/da497cee05acb607ea0e2d225489421146bb6d87/CLAUDE.md
repo: tryethernal/ethernal
kind: claude-md
stars: 267
last_pushed: 2026-06-14T09:13:00Z
license: mit
score: 10
domains: [fullstack, devops, blockchain]
tags: [task-mapping, architectural-rules, environment-constraints, database-operations]
curated: 2026-06-15
curated_by: config-scout
---

# tryethernal/ethernal — claude-md

**Why it's worth keeping:** The 'Task Type' reference table is a superior way to map intent to file locations. Including critical 'gotchas' (like the WebSocket prefix issue) and production database scaling rules prevents common LLM hallucination errors.

**Summary:** A masterclass in providing high-context navigational maps and architectural constraints. It uses a task-based quick reference table to guide an agent through complex system interactions.

**Source credibility:** High; part of an active, well-maintained open-source project with significant star count.

**Recency:** Very current; optimized for modern containerized workflows and agentic reasoning.

**Source:** [tryethernal/ethernal/CLAUDE.md](https://github.com/tryethernal/ethernal/blob/da497cee05acb607ea0e2d225489421146bb6d87/CLAUDE.md) · 267★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Quick Reference

| Task Type | Key Files | Reference |
|-----------|-----------|-----------|
| API endpoint | `run/api/[feature].js`, `run/lib/firebase.js`, `src/plugins/server.js` | [PATTERNS.md](.claude/references/PATTERNS.md) |
| New model | `run/models/`, `run/migrations/`, `run/lib/firebase.js` | [PATTERNS.md](.claude/references/PATTERNS.md) |
| Background job | `run/jobs/[name].js`, `run/jobs/index.js`, `run/lib/queue.js` | [QUEUES.md](.claude/references/QUEUES.md) |
| Frontend component | `src/components/`, `src/stores/`, `src/plugins/router.js` | [PATTERNS.md](.claude/references/PATTERNS.md) |
| Auth/onboarding | `src/components/OnboardingWizard.vue` (unified auth+onboarding), `run/api/onboarding.js`, `run/api/users.js` (signin) | |
| Auth/permissions | `run/middlewares/auth.js`, `run/middlewares/workspaceAuth.js` | |
| L2 integrations | `run/lib/orbit*.js`, `run/lib/op*.js`, `pm2-server/logListener.js` | [L2.md](.claude/references/L2.md) |
| Billing/Stripe | `run/webhooks/stripe.js`, `run/lib/stripe.js`, `run/api/stripe.js` | |
| Testing | `run/tests/mocks/`, `run/tests/api/`, `tests/unit/` | [PATTERNS.md](.claude/references/PATTERNS.md) |
| Database schema
```

</details>
