---
name: 9thLevelSoftware__legion
source: https://github.com/9thLevelSoftware/legion/blob/855e975beec3bac6dc06db598081b6ac11ea8e14/CLAUDE.md
repo: 9thLevelSoftware/legion
kind: claude-md
stars: 62
last_pushed: 2026-05-27T22:24:58Z
license: unknown
score: 9
domains: [ai-agents, cli-tools, project-management]
tags: [multi-agent, orchestration, slash-commands, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# 9thLevelSoftware/legion — claude-md

**Why it's worth keeping:** The 'Mandatory User Interaction Rule' ensures tool-driven communication, while the 'Dynamic Knowledge Index' provides an elite pattern for grounding agent personalities in external markdown files to prevent hallucination.

**Summary:** A highly sophisticated orchestration framework that transforms Claude into a multi-agent project manager via structured slash commands and specialized personas.

**Source credibility:** A niche but highly structured project with moderate social proof (62 stars).

**Recency:** Highly current; explicitly utilizes modern Claude Code tool-calling patterns like AskUserQuestion.

**Source:** [9thLevelSoftware/legion/CLAUDE.md](https://github.com/9thLevelSoftware/legion/blob/855e975beec3bac6dc06db598081b6ac11ea8e14/CLAUDE.md) · 62★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Legion

A multi-CLI plugin for orchestrating 49 AI specialist personalities as a coordinated legion. Works with Claude Code, OpenAI Codex CLI, Cursor, GitHub Copilot CLI, Google Gemini CLI, Antigravity CLI, Kiro CLI, Windsurf, OpenCode, Kilo CLI, and Aider.

## MANDATORY: User Interaction Rule

**When any `/legion:` command needs to ask the user a question or present choices, you MUST use the `AskUserQuestion` tool.** Do NOT output questions as raw text. This applies to every confirmation gate, mode selection, workflow preference, agent swap prompt, and any other user-facing question in any Legion command or skill. No exceptions.

## Available Commands

| Command | Description |
|---------|-------------|
| `/legion:start` | Initialize a new project with guided questioning flow |
| `/legion:plan <N>` | Plan phase N with agent recommendations and wave-structured tasks |
| `/legion:polish` | Polish code for readability, consistency, and clarity (standalone or post-review) |
| `/legion:build` | Execute current phase plans with parallel agent teams |
| `/legion:review` | Run quality review cycle with testing/QA agents |
| `/legion:status` | Show progress dashboard and route to next ac
```

</details>
