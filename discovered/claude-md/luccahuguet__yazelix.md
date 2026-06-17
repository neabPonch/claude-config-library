---
name: luccahuguet__yazelix
source: https://github.com/luccahuguet/yazelix/blob/17da86dee34b006779ec1fe5296085499463c75b/CLAUDE.md
repo: luccahuguet/yazelix
kind: claude-md
stars: 1058
last_pushed: 2026-06-14T04:38:02Z
license: apache-2.0
score: 7
domains: [cli-tools, rust, developer-experience]
tags: [workflow-management, issue-tracking, session-handoff]
curated: 2026-06-14
curated_by: config-scout
---

# luccahuguet/yazelix — claude-md

**Why it's worth keeping:** The 'Session Completion' section offers an excellent template for managing the human-in-the-loop gap, preventing premature pushes of non-trivial changes. It also demonstrates how to explicitly define rules for custom project tooling (Beads).

**Summary:** Provides specific integration for a custom issue tracker and a strict 'Session Completion' protocol to manage hand-offs.

**Source credibility:** High; a highly-starred, actively maintained Rust terminal project.

**Recency:** Current; reflects modern agentic workflow needs like manual verification gates.

**Source:** [luccahuguet/yazelix/CLAUDE.md](https://github.com/luccahuguet/yazelix/blob/17da86dee34b006779ec1fe5296085499463c75b/CLAUDE.md) · 1058★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project Instructions for AI Agents

This file provides instructions and context for AI coding agents working on this project.

<!-- BEGIN BEADS INTEGRATION v:1 profile:minimal hash:ca08a54f -->
## Beads Issue Tracker

This project uses **br (beads_rust)** for issue tracking. Run `br ready` and `br show <id>` for issue context.

### Quick Reference

```bash
br ready              # Find available work
br show <id>          # View issue details
br update <id> --claim  # Claim work
br close <id>         # Complete work
```

### Rules

- Use `br` for ALL task tracking — do NOT use TodoWrite, TaskCreate, or markdown TODO lists
- Keep `.beads/issues.jsonl` tracked as the durable issue state and `.beads/beads.db` ignored as the local cache
- Do not use the retired tracker workflow

## Session Completion

**When ending a work session**, complete the steps below that apply to the current change. For non-trivial changes, local implementation and validation can be complete before push, but remote push must wait until the user manually tests and approves it. Only trivial changes should follow the immediate push path by default.

**MANDATORY WORKFLOW:**

1. **File issues for remaining work** -
```

</details>
