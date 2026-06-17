---
name: majiayu000__vibeguard__claude-example
source: https://github.com/majiayu000/vibeguard/blob/e2d9e973e4a1f718069e9c625cebdc212d2169a0/docs/CLAUDE.md.example
repo: majiayu000/vibeguard
kind: claude-md
stars: 24
last_pushed: 2026-06-16T16:44:10Z
license: mit
score: 9
domains: [agents-ai, devops, security, software-engineering]
tags: [workflow-orchestration, guardrails, verification-driven, reliability]
curated: 2026-06-16
curated_by: config-scout
---

# majiayu000/vibeguard — claude-md

**Why it's worth keeping:** The use of a 'Routing Contract' to decide between planning and execution, combined with specific language-based verification commands, creates highly reliable agent behavior.

**Summary:** A sophisticated operational framework that combines workflow orchestration, multi-layer defensive rules, and automated verification protocols.

**Source credibility:** Highly credible niche tool focused on preventing AI hallucinations/errors; active maintenance.

**Recency:** Very current; utilizes latest Claude Code patterns like subagent isolation and context management.

**Source:** [majiayu000/vibeguard/docs/CLAUDE.md.example](https://github.com/majiayu000/vibeguard/blob/e2d9e973e4a1f718069e9c625cebdc212d2169a0/docs/CLAUDE.md.example) · 24★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — 10x Engineer Configuration

> Integrated Anthropic official best practices + VibeGuard seven-layer defense.
> Different from "recommended compliance" configuration - rules, guard scripts, hooks, and workflow commands provide layered coverage; not every rule is mechanically blocked.

---

## Chat Contract

Compact Chat Contract: progress updates, concise answers, plain formatting.

- Progress updates: for non-trivial or tool-heavy work, send a short update at start, after discovery, before edits, after verification, and when blocked.
- Default verbosity: keep answers concise by default; use short paragraphs for simple tasks and expand only when the work is complex or the user asks for depth.
- Formatting: use Markdown only when it helps; prefer prose first, flat bullets only for natural lists, and avoid decorative structure.

## Workflow Orchestration

### 1. Routing Contract

Follow the canonical router in `workflows/references/routing-contract.md`.

- Precedence: `user_override` → `risk/destructive gate` → `ambiguity gate` → `readiness classifier` → `execution/delegation lane`
- Readiness outputs: `execute_direct`, `plan_first`, `clarify_first`
- Planning handoff key
```

</details>
