---
name: rittmananalytics__wire-plugin
source: https://github.com/rittmananalytics/wire-plugin/blob/640b0f0e3f208416b3aeffc9982bcc4ca03e8435/CLAUDE.md
repo: rittmananalytics/wire-plugin
kind: claude-md
stars: 4
last_pushed: 2026-06-14T20:21:06Z
license: other
score: 9
domains: [agents-ai, cli-tools, workflow-automation]
tags: [framework, agentic-workflow, state-management]
curated: 2026-06-15
curated_by: config-scout
---

# rittmananalytics/wire-plugin — claude-md

**Why it's worth keeping:** It demonstrates expert use of 'Session Start Behavior' for state management and establishes a pattern of mandatory 'generate -> validate -> review' loops to ensure production-grade output.

**Summary:** This file defines a highly structured, command-driven agentic framework that uses slash commands and rigorous validation gates to manage complex project lifecycles.

**Source credibility:** High; comes from a specialized analytics engineering framework with active maintenance.

**Recency:** Very current; specifically tailored for Claude Code's command and status line capabilities.

**Source:** [rittmananalytics/wire-plugin/CLAUDE.md](https://github.com/rittmananalytics/wire-plugin/blob/640b0f0e3f208416b3aeffc9982bcc4ca03e8435/CLAUDE.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Wire Framework — Claude Code Plugin

This plugin provides the **Wire Framework**, an AI-accelerated delivery system for data platform engagements. It encodes 20+ years of analytics engineering methodology as executable workflow specifications, enabling an AI agent to produce production-grade artifacts across the full project lifecycle.

## Session Start Behaviour

At the start of each new conversation (the user's first message), check whether `.wire/` exists in the current directory:

- **`.wire/` exists**: The project has a session-check hook configured. Do not duplicate its output — the hook fires automatically. If for any reason the hook did not fire, output: `[Wire] Run /wire:start to check project status and get next steps.`
- **No `.wire/` directory**: Output a single line before responding to the user's message: `Wire Framework is active — run /wire:start new to start a new engagement, or /wire:adopt if joining a project already in progress.`
- **`.wire/` exists but no releases**: Output: `[Wire] Engagement set up — no releases started yet. Run /wire:new to create your first release.`

Keep these messages to one line. Do not output them on subsequent turns in the same conv
```

</details>
