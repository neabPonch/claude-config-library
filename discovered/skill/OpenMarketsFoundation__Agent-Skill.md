---
name: OpenMarketsFoundation__Agent-Skill
source: https://github.com/OpenMarketsFoundation/Agent-Skill/blob/c9895c6b36c58c171fb6f821bbe6e9591f5d53e5/skill.md
repo: OpenMarketsFoundation/Agent-Skill
kind: skill
stars: 0
last_pushed: 2026-04-13T10:01:26Z
license: unknown
score: 8
domains: [web-frontend, cli-tools, deployment, devops]
tags: [workflow-orchestration, deployment-automation, mode-based-execution]
curated: 2026-06-14
curated_by: config-scout
---

# OpenMarketsFoundation/Agent-Skill — skill

**Why it's worth keeping:** Uses 'Mandatory Mode Selection' to prevent incorrect execution, defines explicit 'Success Gates' for verification, and provides detailed technical constraints for domain-specific logic.

**Summary:** A highly structured operational skill for managing specialized web storefront deployments via mode-based workflows.

**Source credibility:** Low social proof (0 stars), but the high level of domain-specific technical detail suggests a legitimate engineering tool.

**Recency:** Current; updated 2 months ago and utilizes modern agentic workflow patterns.

**Source:** [OpenMarketsFoundation/Agent-Skill/skill.md](https://github.com/OpenMarketsFoundation/Agent-Skill/blob/c9895c6b36c58c171fb6f821bbe6e9591f5d53e5/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Skill: Gamma-Napp Operator

This repository holds the agent skill and operational documentation for Gamma-Napp.
The application code stays in `https://github.com/OpenMarketsFoundation/Store-Front-Nsite`.

## Read First

Before execution, read these sources in this order:

1. `skill.md`
2. `https://github.com/OpenMarketsFoundation/Gamma-Napp/blob/main/AGENTS.md`
3. `https://github.com/OpenMarketsFoundation/Gamma-Napp/blob/main/IMPLEMENTATION_PLAN.md`
4. `https://github.com/OpenMarketsFoundation/Gamma-Napp/blob/main/NSITE%20APP%20INTEGRATION.md`
5. `https://github.com/OpenMarketsFoundation/Gamma-Napp/blob/main/NSITE_DEPLOYMENT_VERIFICATION.md`

If instructions conflict, prefer `skill.md` for execution flow and deployment gates.

## Mandatory First Step: Mode Selection

Before doing anything else, the agent must ask:

"Choose one mode: 1) clone/edit/deploy, 2) rebuild from scratch, 3) clone/deploy existing nsite."

Then run only the selected workflow.

## Mode 1: Clone Gamma-Napp, Edit, Deploy

Use this when code already exists and you want changes shipped quickly.

1. Clone and install:
   - `git clone https://github.com/OpenMarketsFoundation/Store-Front-Nsite.git`
   - `cd Gamma-N
```

</details>
