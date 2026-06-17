---
name: compozy__compozy__skill
source: https://github.com/compozy/compozy/blob/8e99a28c745ce7b1fa0dd400d6748db420c7cae0/skills/compozy/SKILL.md
repo: compozy/compozy
kind: skill
stars: 2282
last_pushed: 2026-06-14T03:22:20Z
license: mit
score: 8
domains: [cli-tools, agents-ai, devops]
tags: [orchestration, workflow, sdlc, automation]
curated: 2026-06-14
curated_by: config-scout
---

# compozy/compozy — skill

**Why it's worth keeping:** It uses a highly structured 'Artifact-Driven' workflow where each phase (PRD -> TechSpec -> Tasks) produces specific documentation required for the next. It also provides explicit 'Do Not Use' constraints to prevent command confusion during transitions.

**Summary:** A high-level orchestration skill that teaches an agent how to manage the full software development lifecycle using the Compozy CLI.

**Source credibility:** High; highly starred and actively maintained repository.

**Recency:** Current; aligns with modern agentic workflow patterns.

**Source:** [compozy/compozy/skills/compozy/SKILL.md](https://github.com/compozy/compozy/blob/8e99a28c745ce7b1fa0dd400d6748db420c7cae0/skills/compozy/SKILL.md) · 2282★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: compozy
description: Explains Compozy capabilities, CLI commands, core workflow skills, optional extension skills, configuration, artifact structure, reusable agents, and extensions. Use when the user asks how to use Compozy, what commands are available, how the workflow pipeline works, or how to configure a workspace. Do not use for executing workflow steps — use the specific cy- skills instead.
---

# Compozy Reference Guide

Comprehensive reference for the Compozy CLI and its AI-assisted development workflow.

## What Is Compozy

Compozy is a Go CLI that orchestrates the full lifecycle of AI-assisted development. It covers product ideation, technical specification, task decomposition, automated execution via AI coding agents, and PR review remediation.

Key characteristics:

- **Agent-agnostic.** Supports claude, codex, copilot, cursor-agent, droid, gemini, opencode, and pi as ACP runtimes.
- **Skills-based.** Bundled skills (installed via `compozy setup`) teach agents how to execute each workflow phase.
- **Artifact-driven.** Planning and review artifacts live as markdown under `.compozy/tasks/<slug>/`, versioned alongside the codebase.
- **Daemon-backed runtime.** A
```

</details>
