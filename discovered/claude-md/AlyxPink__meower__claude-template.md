---
name: AlyxPink__meower__claude-template
source: https://github.com/AlyxPink/meower/blob/ca2818317af70e0eb7de557c1c39223177fa2811/cmd/meower/template/CLAUDE.md.template
repo: AlyxPink/meower
kind: claude-md
stars: 4
last_pushed: 2026-06-07T17:04:46Z
license: agpl-3.0
score: 9
domains: [backend, go, architecture]
tags: [tier-based-rules, sqlc, type-safety]
curated: 2026-06-15
curated_by: config-scout
---

# AlyxPink/meower — claude-md

**Why it's worth keeping:** The semantic coloring of rules provides clear agency boundaries, and the explicit documentation of pattern-specific constraints (like SQLC usage and type-safe routing) prevents common developer errors.

**Summary:** Uses a tiered priority system (Invariant/Default/Preference) to define how an AI should navigate architectural decisions in a multi-module Go project.

**Source credibility:** Part of an opinionated, actively maintained Go framework template.

**Recency:** Highly current; specifically addresses the needs of AI agents working in complex, multi-service environments.

**Source:** [AlyxPink/meower/cmd/meower/template/CLAUDE.md.template](https://github.com/AlyxPink/meower/blob/ca2818317af70e0eb7de557c1c39223177fa2811/cmd/meower/template/CLAUDE.md.template) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Guidance for Claude Code (and other AI agents) working in this repository.

This project was generated from the [Meower](https://github.com/AlyxPink/meower)
template. It's a starting point, not a framework — you're meant to drift from it
freely as the project grows. Update this file as the architecture diverges.

## How to read these rules

- 🔴 **Invariant** — follow without exception. Security, data integrity, cross-layer contracts.
- 🟡 **Default** — follow unless the current task has a specific reason not to. State the reason briefly if you deviate.
- 🟢 **Preference** — apply when it serves the task. Judgment call.

Words like "always", "never", "must" inside a 🟡 or 🟢 rule describe the
*default*, not an absolute. If uncertain, ask.

## Stack & Structure

| Layer | Tech |
|-------|------|
| Web | Fiber + Templ + HTMX + TailwindCSS |
| API | Go + gRPC + PostgreSQL (SQLC) |
| Observability | OpenTelemetry + Prometheus + structured logs (charmbracelet/log) |
| Dev | Docker Compose + `wgo` (hot reload) |

**Flow**: Browser → Web (Fiber) → gRPC → API → PostgreSQL

This is a multi-module Go workspace (a root `go.work` ties the modules
together):

```
TEMPLATE_PROJECT_NAME/
```

</details>
