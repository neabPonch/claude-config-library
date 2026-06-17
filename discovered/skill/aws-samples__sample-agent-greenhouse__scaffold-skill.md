---
name: aws-samples__sample-agent-greenhouse__scaffold-skill
source: https://github.com/aws-samples/sample-agent-greenhouse/blob/39f216dea23ed758da3c404d18db9bc9314fb40d/docs/design/scaffold-skill.md
repo: aws-samples/sample-agent-greenhouse
kind: skill
stars: 21
last_pushed: 2026-05-19T07:57:16Z
license: mit-0
score: 8
domains: [agents-ai, software-architecture, devops]
tags: [scaffolding, project-generation, production-ready]
curated: 2026-06-15
curated_by: config-scout
---

# aws-samples/sample-agent-greenhouse — skill

**Why it's worth keeping:** It defines a rigorous 'Platform Readiness' checklist (C1-C12) to ensure generated code includes essential operational features like health checks, logging, and graceful shutdowns. The template implementation strategy using string constants is also highly portable for skill design.

**Summary:** A design document for a scaffolding skill that generates production-ready agent project skeletons across various architectures.

**Source credibility:** High; comes from an official AWS sample repository.

**Recency:** Extremely current (pushed 1 month ago).

**Source:** [aws-samples/sample-agent-greenhouse/docs/design/scaffold-skill.md](https://github.com/aws-samples/sample-agent-greenhouse/blob/39f216dea23ed758da3c404d18db9bc9314fb40d/docs/design/scaffold-skill.md) · 21★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Scaffold Skill — Design Document

## Purpose

The `scaffold` skill pack augments the Foundation Agent with project generation
capabilities. When loaded, the agent becomes a "Project Scaffolder" that can create
complete, runnable agent project skeletons following platform best practices.

**Core question this skill answers:** "Give me a working starting point for my agent
project that already follows all platform requirements."

## Developer Pain Points Addressed

1. **"How do I structure my agent project?"** — Developers shouldn't have to reverse-
   engineer project structure from documentation. The Scaffold skill generates it.
2. **"What boilerplate do I need?"** — Dockerfile, health checks, logging setup,
   graceful shutdown — all included from the start.
3. **"Will this pass platform checks?"** — Generated projects are designed to achieve
   a READY rating from the Design Advisor skill (0 blockers, ≤2 warnings).

## Template Types

The Scaffold skill supports four project templates, each targeting a different
agent architecture:

| Template | Description | Use Case |
|----------|-------------|----------|
| `basic-agent` | Single Foundation Agent with health check and HTTP se
```

</details>
