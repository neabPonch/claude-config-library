---
name: Kilo59__ruff-sync__agent-skill
source: https://github.com/Kilo59/ruff-sync/blob/28f4259535b2911bafb8a2dc730dc2fdc88901bb/docs/agent-skill.md
repo: Kilo59/ruff-sync
kind: skill
stars: 4
last_pushed: 2026-06-09T21:13:04Z
license: mit
score: 9
domains: [cli-tools, devops]
tags: [progressive-disclosure, structured-knowledge, agent-orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# Kilo59/ruff-sync — skill

**Why it's worth keeping:** It implements progressive disclosure by using a concise entry point (SKILL.md) and specific reference files, preventing context bloat while allowing deep dives when necessary.

**Summary:** A high-quality skill architecture that uses a hub-and-spoke documentation model for specialized CLI tool expertise.

**Source credibility:** Well-structured implementation following the emerging agentskills.io specification.

**Recency:** Highly current; optimizes for modern LLM token constraints via structured tool discovery.

**Source:** [Kilo59/ruff-sync/docs/agent-skill.md](https://github.com/Kilo59/ruff-sync/blob/28f4259535b2911bafb8a2dc730dc2fdc88901bb/docs/agent-skill.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Agent Skill

`ruff-sync` ships an [Agent Skill](https://agentskills.io/home) — a structured, machine-readable file that teaches AI coding agents how to adopt and operate the tool. Any [Agent Skills–compatible](https://agentskills.io/what-are-skills) agent (GitHub Copilot, Claude Code, Cursor, etc.) will automatically discover and use it when working on your project.

## What Is an Agent Skill?

The [Agent Skills specification](https://agentskills.io/specification) is an open format for packaging domain expertise as a `SKILL.md` file. Agents load it when the task is relevant, gaining specialized knowledge without you needing to re-explain it every time.

## What the ruff-sync Skill Covers

The skill lives at [`.agents/skills/ruff-sync-usage/`](https://github.com/Kilo59/ruff-sync/tree/main/.agents/skills/ruff-sync-usage/) and teaches agents:

| File | Contents |
|---|---|
| `SKILL.md` | Quick start, persistent config, common workflows, exit codes, and gotchas |
| `references/configuration.md` | Full `[tool.ruff-sync]` key reference |
| `references/troubleshooting.md` | Common errors and how to resolve them |
| `references/ci-integration.md` | GitHub Actions, GitLab CI, pre-commit,
```

</details>
