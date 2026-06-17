---
name: SteelMorgan__cursor-anthropic-skills__go-skill
source: https://github.com/SteelMorgan/cursor-anthropic-skills/blob/4df7122c0960d54fe1b9a7e535cc92c315cee653/custom-skills/GO_SKILL.md
repo: SteelMorgan/cursor-anthropic-skills
kind: skill
stars: 26
last_pushed: 2026-03-24T08:28:50Z
license: mit
score: 9
domains: [backend-api, microservices, observability]
tags: [go, clean-architecture, opentelemetry, expert-guide]
curated: 2026-06-15
curated_by: config-scout
---

# SteelMorgan/cursor-anthropic-skills — skill

**Why it's worth keeping:** Includes highly specific code patterns for error wrapping, table-driven testing, and OpenTelemetry tracing. The pre-development checklist provides actionable guardrails for the agent.

**Summary:** A production-grade guide for Go backend development focusing on Clean Architecture, microservices, and observability.

**Source credibility:** Respectable specialized repository with recent activity.

**Recency:** Highly relevant to current Go development standards.

**Source:** [SteelMorgan/cursor-anthropic-skills/custom-skills/GO_SKILL.md](https://github.com/SteelMorgan/cursor-anthropic-skills/blob/4df7122c0960d54fe1b9a7e535cc92c315cee653/custom-skills/GO_SKILL.md) · 26★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: go-development-expert
description: Expert guide for Go development with Clean Architecture, microservices patterns, and OpenTelemetry observability. Use when writing, reviewing, or refactoring Go code, implementing microservices, or setting up observability with distributed tracing.
enforcement_level: HIGH
violation_consequence: Code may violate best practices, lack proper error handling, or miss critical observability instrumentation leading to production issues
---

# Go Development Expert

You are an expert in Go, microservices architecture, and clean backend development practices. Your role is to ensure code is idiomatic, modular, testable, and aligned with modern best practices and design patterns.

## ✓ Pre-Development Checklist

Before writing Go code:
- [ ] Project structure follows standard layout (cmd/, internal/, pkg/)
- [ ] Dependencies use Go modules (go.mod present)
- [ ] Error handling strategy defined
- [ ] Context propagation planned for all operations
- [ ] Observability requirements identified

## General Responsibilities

- Guide the development of idiomatic, maintainable, and high-performance Go code
- Enforce modular design and separation of concerns
```

</details>
