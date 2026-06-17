---
name: microsoft__TypeAgent__claude
source: https://github.com/microsoft/TypeAgent/blob/3d6af4fbf8c1941877d71e910be2718ab9fd3bf6/ts/packages/agents/powershell/CLAUDE.md
repo: microsoft/TypeAgent
kind: claude-md
stars: 707
last_pushed: 2026-06-14T08:13:15Z
license: mit
score: 9
domains: [agents-ai, cli-tools, devops]
tags: [powershell, agent-architecture, schema-definitions]
curated: 2026-06-15
curated_by: config-scout
---

# microsoft/TypeAgent — claude-md

**Why it's worth keeping:** Excellent use of structured data schemas and grammar syntax definitions to bridge high-level architectural intent with low-level implementation requirements.

**Summary:** Defines the architecture, lifecycle, and exact JSON schema for a PowerShell-based agentic component within TypeAgent.

**Source credibility:** High; part of a Microsoft research repository exploring agent orchestration.

**Recency:** Extremely current, as evidenced by the zero-month-old push date.

**Source:** [microsoft/TypeAgent/ts/packages/agents/powershell/CLAUDE.md](https://github.com/microsoft/TypeAgent/blob/3d6af4fbf8c1941877d71e910be2718ab9fd3bf6/ts/packages/agents/powershell/CLAUDE.md) · 707★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# PowerShell Agent — Claude Code Instructions

PowerShell captures and reuses PowerShell scripts from reasoning traces.
Scripts persist in instance storage (`~/.typeagent/profiles/<profile>/powershell/`)
across sessions. Grammar rules are registered dynamically at runtime — no build
step needed for user-created flows.

---

## Architecture

- **Instance storage**: flows + scripts persist across sessions via `SessionContext.instanceStorage`
- **Runtime grammar registration**: `.agr` rule text → `globalAgentGrammarRegistry.addGeneratedRules()`
- **Sample seeding**: `samples/*.recipe.json` are copied to instance storage on first activation
- **Build-time compilation** (`compileRecipes.mjs`): only for developer workflow, not production

## Storage Layout (in instance storage)

```
powershell/
├── index.json                  # Flow registry index
├── flows/
│   └── listFiles.flow.json     # Flow metadata + parameters + sandbox
├── scripts/
│   └── listFiles.ps1           # Separated PowerShell script
└── pending/
    └── *.recipe.json           # Captured from reasoning, not yet promoted
```

## Lifecycle

1. `updateAgentContext(enable=true)` → init store → seed samples → register gramm
```

</details>
