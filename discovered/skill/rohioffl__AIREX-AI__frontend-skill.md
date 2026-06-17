---
name: rohioffl__AIREX-AI__frontend-skill
source: https://github.com/rohioffl/AIREX-AI/blob/0def2b260e34f070bade28b98aca660c0f081c7e/docs/frontend_skill.md
repo: rohioffl/AIREX-AI
kind: skill
stars: 0
last_pushed: 2026-06-15T12:19:53Z
license: other
score: 9
domains: [web-frontend, sre-ops, real-time-systems]
tags: [state-machine, sse, dashboard, safety-first]
curated: 2026-06-16
curated_by: config-scout
---

# rohioffl/AIREX-AI — skill

**Why it's worth keeping:** It provides an explicit backend state machine and 'Strict Prohibitions' that prevent the AI from implementing dangerous patterns like optimistic UI or hardcoded business logic. The technical depth in defining event handlers for SSE makes it a masterclass in building deterministic, reactive UIs.

**Summary:** A highly rigorous specification for building a mission-critical, state-driven SRE dashboard using real-time SSE updates.

**Source credibility:** Low public social proof (0 stars), but the high density of specific architectural constraints indicates a professional engineering spec.

**Recency:** Very current, explicitly targeting React 19 and modern real-time patterns.

**Source:** [rohioffl/AIREX-AI/docs/frontend_skill.md](https://github.com/rohioffl/AIREX-AI/blob/0def2b260e34f070bade28b98aca660c0f081c7e/docs/frontend_skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: frontend-sre-dashboard
description: Build a production-grade, state-driven SRE dashboard for the Agentic AI Incident Response Platform. Focus on operational clarity, real-time updates (SSE), and strict backend state adherence.
license: Private
---

# Frontend Skill — AIREX

> **Multi-organization note:** **`AuthContext`** exposes **`organizations`**, **`tenants`**, **`active_tenant`**, and **`active_organization`** from `/auth/me`. Users switch workspaces via **`switchTenant`** (persists active tenant and refreshes session). Platform operators use **`PlatformAdminPage`** and related **`/admin/*`** routes. API calls must send the active tenant when the backend expects it (see Axios defaults in `apps/web/src/services/api.js`).

This skill defines the frontend implementation rules for the operational SRE dashboard.

This is NOT a marketing site.
This is NOT a generic admin panel.
This is an operational control surface for incident management.

The UI must be:

- **State-driven**: Render strictly based on backend state.
- **Dark-themed**: Default to dark mode for operational use.
- **Deterministic**: Same state = Same UI, always.
- **Safe**: Prevent accidental execution.
- **
```

</details>
