---
name: mk-knight23__AGENTS-COLLECTION__customize-skill
source: https://github.com/mk-knight23/AGENTS-COLLECTION/blob/41d09336e6aa7f881389b585edfb34768b0a8ca3/DOCS/.CLAUDE/customize-SKILL.md
repo: mk-knight23/AGENTS-COLLECTION
kind: skill
stars: 72
last_pushed: 2026-04-16T07:24:00Z
license: unknown
score: 8
domains: [agents-ai, system-architecture, cli-tools]
tags: [customization, architectural-context, workflow]
curated: 2026-06-16
curated_by: config-scout
---

# mk-knight23/AGENTS-COLLECTION — skill

**Why it's worth keeping:** The use of a file-to-purpose mapping table and prescriptive 'Implementation Patterns' eliminates AI guesswork during complex refactors.

**Summary:** Provides high-density architectural context and implementation patterns for modifying the NanoClaw agent system.

**Source credibility:** Relatively strong with 72 stars and recent activity (2 months ago).

**Recency:** Current, following modern agentic workflows.

**Source:** [mk-knight23/AGENTS-COLLECTION/DOCS/.CLAUDE/customize-SKILL.md](https://github.com/mk-knight23/AGENTS-COLLECTION/blob/41d09336e6aa7f881389b585edfb34768b0a8ca3/DOCS/.CLAUDE/customize-SKILL.md) · 72★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: customize
description: Add new capabilities or modify NanoClaw behavior. Use when user wants to add channels (Telegram, Slack, email input), change triggers, add integrations, modify the router, or make any other customizations. This is an interactive skill that asks questions to understand what the user wants.
---

# NanoClaw Customization

This skill helps users add capabilities or modify behavior. Use AskUserQuestion to understand what they want before making changes.

## Workflow

1. **Understand the request** - Ask clarifying questions
2. **Plan the changes** - Identify files to modify
3. **Implement** - Make changes directly to the code
4. **Test guidance** - Tell user how to verify

## Key Files

| File | Purpose |
|------|---------|
| `src/index.ts` | Orchestrator: state, message loop, agent invocation |
| `src/channels/whatsapp.ts` | WhatsApp connection, auth, send/receive |
| `src/ipc.ts` | IPC watcher and task processing |
| `src/router.ts` | Message formatting and outbound routing |
| `src/types.ts` | TypeScript interfaces (includes Channel) |
| `src/config.ts` | Assistant name, trigger pattern, directories |
| `src/db.ts` | Database initialization and queries
```

</details>
