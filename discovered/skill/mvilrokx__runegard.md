---
name: mvilrokx__runegard
source: https://github.com/mvilrokx/runegard/blob/fddd8c04d026e2fa777d2a6dd6340cb7ad95a324/skill.md
repo: mvilrokx/runegard
kind: skill
stars: 5
last_pushed: 2026-03-08T03:50:46Z
license: unknown
score: 8
domains: [devops, kubernetes, cli-tools, agents-ai]
tags: [k8s, runbook, automation, reliability-engineering]
curated: 2026-06-14
curated_by: config-scout
---

# mvilrokx/runegard — skill

**Why it's worth keeping:** The categorical distinction between diagnostic and remediation steps creates a highly effective safety guardrail for agentic actions. The integration of an 'improve' phase provides a clear pattern for building local, file-based persistent memory from execution traces.

**Summary:** An autonomous Kubernetes operations tool that converts markdown runbooks into executable decision trees with human-in-the-loop safety checks. It features a continuous learning loop to refine execution patterns based on trace logs.

**Source credibility:** Niche tool with modest star count that demonstrates high technical specificity.

**Recency:** Very current; uses modern Python tooling (uv) and fits contemporary agentic workflows.

**Source:** [mvilrokx/runegard/skill.md](https://github.com/mvilrokx/runegard/blob/fddd8c04d026e2fa777d2a6dd6340cb7ad95a324/skill.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: runegard
description: >
  Autonomous runbook executor for Kubernetes operations. Reads markdown runbooks,
  parses them into executable decision trees, and follows them step-by-step
  against a live K8s cluster. Requests human approval before any mutating action.
  Includes an CL-powered improvement loop that learns from execution failures.
---

# RuneGärd -- Kubernetes Runbook Executor

## When to Use This Skill

Use this skill when:
- You have a runbook document describing an operational procedure
- You need to diagnose or remediate a Kubernetes issue
- You want to follow a step-by-step troubleshooting guide against a live cluster

## Workflow

### Phase 1: Parse the Runbook

1. Accept a runbook file path from the user
2. Run: `uv run python -m runegard parse <runbook_path>`
3. Present the parsed structure to the user for confirmation:
   - Number of steps detected
   - Decision points identified
   - Commands that will be executed
4. If the user wants changes, adjust and re-parse

### Phase 2: Execute the Runbook

1. Ask the user for execution mode:
   - Interactive (default): pause before remediation steps for approval
   - Dry-run: walk the tree without executing any
```

</details>
