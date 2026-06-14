---
name: ApiwatKansaard__Claude_QA_Agent
source: https://github.com/ApiwatKansaard/Claude_QA_Agent/blob/7b1cd061138c7e0e62d3ae6f81d910704b98ffa0/CLAUDE.md
repo: ApiwatKansaard/Claude_QA_Agent
kind: claude-md
stars: 1
last_pushed: 2026-06-11T09:42:32Z
license: unknown
score: 9
domains: [qa-automation, agents-ai, devops]
tags: [multi-agent, slash-commands, structured-constraints]
curated: 2026-06-14
curated_by: config-scout
---

# ApiwatKansaard/Claude_QA_Agent — claude-md

**Why it's worth keeping:** The 'Team QA Rules' section is masterclass level; it uses hyper-specific negative/positive constraints (e.g., Jira field IDs, avoiding `wc -l` for CSVs) to prevent common agent failure modes. It demonstrates how to encode domain-specific business logic and tool protocols directly into the instructions.

**Summary:** This config sets up a multi-role QA agent system using slash commands to orchestrate test planning, automation, and reporting. It includes high-level role definitions and specific tool integration workflows.

**Source credibility:** Low star count, but the highly specific technical constraints suggest a high-maturity internal workflow.

**Recency:** Current; utilizes modern automation patterns like Playwright and structured CLI interactions.

**Source:** [ApiwatKansaard/Claude_QA_Agent/CLAUDE.md](https://github.com/ApiwatKansaard/Claude_QA_Agent/blob/7b1cd061138c7e0e62d3ae6f81d910704b98ffa0/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# QA Ops Director — Claude Code Project

AI-powered QA assistant for test planning, bug triage, TestRail management, and QA reporting.
Runs on **Claude Code** (CLI + VSCode Extension) and **GitHub Copilot** (lite mode).

## First time? Run: `/qa-get-started`

The onboarding wizard will install everything, configure credentials, verify tools, and run your first test — all interactively. Works on both Claude Code and Copilot.

## How to use

Use slash commands (e.g., `/qa-test-plan`) or describe your task in natural language.
Claude will route to the correct workflow automatically.

## Agent roster

- **qa-ops-director** — QA Lead: test plans, AC writing, bug reports, TestRail, standups
- **playwright-automator** — Automation Engineer: generate/run/review Playwright tests
- **automation-reviewer** — Code Reviewer: review test quality and detect conflicts

## Full routing and workflow details

Read `.github/skills/qa-ops-director/SKILL.md` for:
- Complete slash command routing table (16 commands)
- Auto-chain pipeline details (/qa-test-plan, /qa-write-ac)
- Tool integrations (Jira, Confluence, Figma, TestRail, Gmail, Calendar)

Read `.github/skills/playwright-automator/SKILL.md` for:
```

</details>
