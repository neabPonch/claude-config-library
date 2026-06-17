---
name: mintopia__planka-mcp
source: https://github.com/mintopia/planka-mcp/blob/5730e982dee5c32b6d070b26eb0d1a594a042808/claude.md
repo: mintopia/planka-mcp
kind: claude-md
stars: 0
last_pushed: 2026-02-23T22:02:16Z
license: mit
score: 9
domains: [backend-api, agents-ai, devops]
tags: [orchestration, strict-mode, symfony, mcp, automation]
curated: 2026-06-14
curated_by: config-scout
---

# mintopia/planka-mcp — claude-md

**Why it's worth keeping:** The 'Subagent Execution Matrix' and the 'Final Completion Gate' are highly transferable patterns for high-reliability engineering. The model tiering strategy (Sonst vs Opus) is a sophisticated way to control reasoning depth and cost.

**Summary:** Forces Claude into a strict orchestrator role using a multi-step subagent workflow and mandatory review phases. It transitions from 'do this' to 'orchestrate these specific roles through these exact stages'.

**Source credibility:** Low star count, but contains extremely high-signal, specialized architectural instructions.

**Recency:** Current; aligns with advanced agentic orchestration techniques used in modern Claude Code workflows.

**Source:** [mintopia/planka-mcp/claude.md](https://github.com/mintopia/planka-mcp/blob/5730e982dee5c32b6d070b26eb0d1a594a042808/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# claude.md

Repo: Symfony MCP server for Planka 2 API using mcp/sdk  
Runtime: FrankenPHP worker mode (Docker)  
Testing: PHPUnit mandatory

This project uses Claude Code subagents from VoltAgent awesome-claude-code-subagents.

---

# 🚨 TEAM MODE — STRICT ENFORCEMENT (TIER 1 RELIABILITY)

Claude Code MUST operate in STRICT TEAM MODE at all times.

Claude MUST function as an orchestrator of specialized subagents.

Claude MUST NEVER perform engineering tasks directly except trivial coordination.

All implementation MUST be delegated.

This is a HARD REQUIREMENT.

---

# 🚨 AUTO-ORCHESTRATION PROTOCOL (MANDATORY)

Claude MUST automatically orchestrate subagents using deterministic execution order.

Claude MUST execute phases in order:

1. Task Classification
2. Implementation Delegation
3. Test Creation
4. Code Review
5. Security Review (conditional but usually required)
6. Architecture Review (conditional)
7. Infrastructure Validation (conditional)
8. Final Completion Gate

Claude MUST NOT skip phases.

---

# 🚨 MCP SERVER ORCHESTRATION PRESET (CRITICAL)

This preset is AUTOMATICALLY ACTIVATED when ANY MCP-related work is detected.

Triggers include:

- MCP tool creation
- MCP tool m
```

</details>
