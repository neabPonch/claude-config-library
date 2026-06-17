---
name: iamtouchskyer__opc
source: https://github.com/iamtouchskyer/opc/blob/6b35d667a21ead52d594560edfb2fb403fc93222/skill.md
repo: iamtouchskyer/opc
kind: skill
stars: 170
last_pushed: 2026-06-14T03:50:52Z
license: mit
score: 9
domains: [agents-ai, software-engineering, cli-tools]
tags: [orchestrator, workflow-engine, multi-role, quality-assurance]
curated: 2026-06-14
curated_by: config-scout
---

# iamtouchskyer/opc — skill

**Why it's worth keeping:** The principle of separating execution from evaluation via multi-stage 'gate' protocols is highly transferable. The structured flow templates (e.g., build-verify, full-stack) provide a blueprint for high-reliability autonomous development.

**Summary:** A sophisticated agent orchestration framework that uses a digraph engine to move tasks through specialized roles and quality gates. It implements an 'adversarial' approach where the agent performing work is never the one evaluating it.

**Source credibility:** High; 170 stars and very recent updates suggest a well-regarded and active project.

**Recency:** Current; utilizes modern session/state management patterns suitable for advanced Claude Code usage.

**Source:** [iamtouchskyer/opc/skill.md](https://github.com/iamtouchskyer/opc/blob/6b35d667a21ead52d594560edfb2fb403fc93222/skill.md) · 170★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: opc
version: 0.10.2
description: "OPC — One Person Company. Digraph-based task pipeline with independent multi-role evaluation. Builds, reviews, analyzes, and brainstorms with specialist agents. Every path ends with evaluation. /opc <task>, /opc -i <task>, /opc <role> [role...]"
---

# OPC — One Person Company

One principle: **the agent that does the work never evaluates it.**

A full team in a single skill. The digraph engine handles any task — building code, reviewing code, analyzing problems, brainstorming designs. It infers which flow and entry point to use from the task itself, and every path ends with independent evaluation.

## Invocation

**Harness path:** The `opc-harness` binary lives at `bin/opc-harness.mjs` relative to this skill's install directory. Resolve it once at session start:
```bash
OPC_HARNESS="$HOME/.claude/skills/opc/bin/opc-harness.mjs"
```
All `opc-harness` references below mean `node "$OPC_HARNESS"`. Set this as a shell variable and reuse it throughout the session.

```
/opc <task>              # auto mode — infer flow and roles from the task
/opc -i <task>           # interactive mode — ask questions before dispatch
/opc <role> [role...]    #
```

</details>
