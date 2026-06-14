---
name: zakirkun__guardian-cli
source: https://github.com/zakirkun/guardian-cli/blob/68f79f80023ecbda97a42559a07db234776203de/SKILL.md
repo: zakirkun/guardian-cli
kind: skill
stars: 1450
last_pushed: 2026-05-29T03:17:39Z
license: other
score: 9
domains: [agents-ai, cli-tools, security, automation]
tags: [multi-agent, orchestration, workflow-engine, security-automation]
curated: 2026-06-14
curated_by: config-scout
---

# zakirkun/guardian-cli — skill

**Why it's worth keeping:** The separation of concerns between Planner, ToolAgent, and Analyst roles is a top-tier pattern; specifically, the use of 'PentestMemory' to link raw tool executions to interpreted findings provides essential traceability for agentic workflows.

**Summary:** An architectural blueprint for a multi-agent security orchestration CLI that uses role-based agents and structured state management.

**Source credibility:** High; 1450 stars and recent updates indicate a widely adopted, production-ready tool.

**Recency:** Current; uses modern AI provider abstractions and high-level orchestration logic suitable for today's LLMs.

**Source:** [zakirkun/guardian-cli/SKILL.md](https://github.com/zakirkun/guardian-cli/blob/68f79f80023ecbda97a42559a07db234776203de/SKILL.md) · 1450★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: guardian-cli
description: >
  An enterprise-grade, AI-powered penetration testing automation CLI tool.
  Orchestrates multiple specialized AI agents (Planner, ToolAgent, Analyst, Reporter)
  backed by 4 AI providers (OpenAI, Claude, Gemini, OpenRouter) and 19 integrated
  security tools through YAML-defined workflows. Produces professional Markdown, HTML,
  or JSON security reports with full evidence capture and traceability.
---

# Guardian CLI – Skill Reference

## 1. Project Overview

**Guardian** (v2.0) is a Python 3.11+ CLI application that automates penetration testing workflows using a multi-agent AI system. It is designed for **authorized** security assessments only.

```
guardian-cli/
├── ai/               # AI provider integrations & prompt templates
│   ├── providers/    # base_provider, openai, claude, gemini, openrouter
│   └── prompt_templates/
├── cli/              # CLI entry-point (Typer) & commands
│   └── commands/     # init, scan, recon, analyze, report, workflow, ai, models
├── core/             # Multi-agent orchestration engine
│   ├── agent.py          # BaseAgent
│   ├── planner.py        # PlannerAgent  – decides next test step
│   ├── tool_agen
```

</details>
