---
name: opensandbox-group__OpenSandbox
source: https://github.com/opensandbox-group/OpenSandbox/blob/40948c070b47f4d20b38518774ab40ded685ae21/CLAUDE.md
repo: opensandbox-group/OpenSandbox
kind: claude-md
stars: 11537
last_pushed: 2026-06-15T16:22:14Z
license: apache-2.0
score: 9
domains: [infrastructure, monorepo, systems-programming, cloud-native]
tags: [hierarchical-rules, guardrails, spec-driven, monorepo]
curated: 2026-06-15
curated_by: config-scout
---

# opensandbox-group/OpenSandbox — claude-md

**Why it's worth keeping:** The 'Ask first' and 'Never' guardrails are highly actionable for preventing destructive refactoring in large systems. The pattern of prioritizing specification-driven development is excellent for tool-use stability.

**Summary:** Uses a hierarchical AGENTS.md routing system to manage rule scoping across a complex monorepo. It focuses heavily on keeping public contracts (specs, SDKs, CLI) aligned with implementations.

**Source credibility:** High: the source is a popular, actively maintained infrastructure project (11k+ stars).

**Recency:** Current: matches the needs of modern agentic workflows and Claude Code's capabilities.

**Source:** [opensandbox-group/OpenSandbox/CLAUDE.md](https://github.com/opensandbox-group/OpenSandbox/blob/40948c070b47f4d20b38518774ab40ded685ae21/CLAUDE.md) · 11537★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# OpenSandbox Claude Guide

Use this file as the Claude Code entry point for the OpenSandbox monorepo. Treat `AGENTS.md` as the canonical router and prefer the nearest local `AGENTS.md` for task-specific rules.

## Read First

- Root rules: `AGENTS.md`
- Server changes: `server/AGENTS.md`
- SDK changes: `sdks/AGENTS.md`
- Spec changes: `specs/AGENTS.md`
- Kubernetes changes: `kubernetes/AGENTS.md`
- Areas without a local `AGENTS.md`: read the nearest `README.md`, `DEVELOPMENT.md`, and relevant CI workflow.

## Repository Map

- `server/`: FastAPI lifecycle control plane, Docker/Kubernetes runtime integration, snapshot metadata, and server tests
- `components/execd/`: in-sandbox execution daemon
- `components/egress/`: per-sandbox network egress policy sidecar
- `components/ingress/`: ingress gateway and endpoint routing
- `sdks/`: sandbox, code-interpreter, and MCP SDKs plus generated clients
- `specs/`: public OpenAPI contracts and examples
- `kubernetes/`: Kubernetes operator, CRDs, task-executor, Helm charts, and Kind e2e tests
- `cli/`: `osb` command-line client and bundled CLI skills
- `tests/`: cross-language end-to-end SDK tests
- `docs/`, `examples/`, `sandboxes/`, `oseps/`
```

</details>
