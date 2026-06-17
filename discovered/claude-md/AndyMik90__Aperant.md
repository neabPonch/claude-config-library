---
name: AndyMik90__Aperant
source: https://github.com/AndyMik90/Aperant/blob/20250db069a849ab001ac6ab9e3e9779886ab9e2/CLAUDE.md
repo: AndyMik90/Aperant
kind: claude-md
stars: 14357
last_pushed: 2026-06-14T08:27:00Z
license: agpl-3.0
score: 9
domains: [agents-ai, desktop-app, typescript, electron]
tags: [orchestration, guardrails, workflow-pattern, troubleshooting]
curated: 2026-06-15
curated_by: config-scout
---

# AndyMik90/Aperant — claude-md

**Why it's worth keeping:** The <orchestrator_pattern> provides an excellent template for multi-agent workflow control, while the detailed 'Known Gotchas' section offers practical operational recovery steps.

**Summary:** Defines strict architectural guardrails and a high-level 'Orchestrator' behavioral pattern for complex task delegation.

**Source credibility:** Highly credible; high star count and recent activity indicate a major, well-maintained autonomous agent project.

**Recency:** Very current, utilizing modern patterns like Vercel AI SDK v6 and advanced agentic workflows.

**Source:** [AndyMik90/Aperant/CLAUDE.md](https://github.com/AndyMik90/Aperant/blob/20250db069a849ab001ac6ab9e3e9779886ab9e2/CLAUDE.md) · 14357★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code when working with this repository.

Auto Claude is an autonomous multi-agent coding framework that plans, builds, and validates software for you. It's a TypeScript-first Electron desktop application with a self-contained AI agent layer (Vercel AI SDK v6). A lightweight Python sidecar provides the optional Graphiti memory system.

> **Deep-dive reference:** [ARCHITECTURE.md](shared_docs/ARCHITECTURE.md) | **Frontend contributing:** [apps/desktop/CONTRIBUTING.md](apps/desktop/CONTRIBUTING.md)

## Product Overview

Auto Claude is a desktop application (+ CLI) where users describe a goal and AI agents autonomously handle planning, implementation, and QA validation. All work happens in isolated git worktrees so the main branch stays safe.

**Core workflow:** User creates a task → Spec creation pipeline assesses complexity and writes a specification → Planner agent breaks it into subtasks → Coder agent implements (can spawn parallel subagents) → QA reviewer validates → QA fixer resolves issues → User reviews and merges.

**Main features:**

- **Autonomous Tasks** — Multi-agent pipeline (planner, coder, QA) that builds features end-t
```

</details>
