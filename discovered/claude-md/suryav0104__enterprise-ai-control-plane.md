---
name: suryav0104__enterprise-ai-control-plane
source: https://github.com/suryav0104/enterprise-ai-control-plane/blob/447834dbb207df311f655011a1446e180cfb117b/claude.md
repo: suryav0104/enterprise-ai-control-plane
kind: claude-md
stars: 0
last_pushed: 2026-04-10T23:04:57Z
license: unknown
score: 8
domains: [agents-ai, cli-tools, software-architecture]
tags: [workflow-enforcement, plugin-architecture, agentic-orchestration]
curated: 2026-06-14
curated_by: config-scout
---

# suryav0104/enterprise-ai-control-plane — claude-md

**Why it's worth keeping:** The mandatory documentation/diagram phase prevents premature implementation, while the specific component discovery patterns (agents/commands/skills) provide a clear blueprint for organization and scale.

**Summary:** Enforces an 'Architecture-First' workflow and provides strict structural rules for building agentic plugin components.

**Source credibility:** Low social proof due to 0 stars, but the technical specificity of the rules suggests high-quality intent.

**Recency:** Highly current; specifically addresses Claude Code plugin structures.

**Source:** [suryav0104/enterprise-ai-control-plane/claude.md](https://github.com/suryav0104/enterprise-ai-control-plane/blob/447834dbb207df311f655011a1446e180cfb117b/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Enterprise AI Control Plane — Project Instructions

## Project Overview
Monorepo for an enterprise AI governance platform built as a Claude Code plugin.
Display name: "Enterprise AI Control Plane"
Folder should be renamed to: `enterprise-ai-control-plane`

## Phases
- **Phase 1:** Agent Orchestration (current) — `/rca` command with 4-agent pipeline
- **Phase 2:** Guardrails Layer — input/output validation, policy engine
- **Phase 3:** Evaluation Framework — metrics, benchmarks, red-teaming
- **Phase 4:** Observability Dashboard — audit logs, usage, cost, failures

## Architecture-First Rule
**Do not write any implementation code until:**
1. `docs/architecture.md` has been created and reviewed by the user
2. Excalidraw diagram has been generated and reviewed by the user

## Memory
Save memory at the end of every session covering: what was built, decisions made, current status, next steps.

## New Components
All new platform components go in their own subfolder (guardrails/, evaluation/, observability/).
Never mix components — each subfolder is self-contained.

## Plugin Structure
This is a Claude Code plugin. Key conventions:
- `plugin.json` is metadata only — no agent/command/ski
```

</details>
