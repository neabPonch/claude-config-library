---
name: mshogin__archlint
source: https://github.com/mshogin/archlint/blob/47b46954dcdf14f8ed8edc897410890f9c7c3686/CLAUDE.md
repo: mshogin/archlint
kind: claude-md
stars: 23
last_pushed: 2026-06-14T00:32:34Z
license: apache-2.0
score: 8
domains: [cli-tools, backend, go]
tags: [agentic-workflow, maintainer-rules, architecture-enforcement]
curated: 2026-06-14
curated_by: config-scout
---

# mshogin/archlint — claude-md

**Why it's worth keeping:** Provides excellent templates for 'agentic' workflows like periodic task checks, structured communication protocols via GitHub issues, and strict architectural constraints (e.g., interface method limits).

**Summary:** Defines high-agency behaviors where Claude acts as a proactive maintainer rather than just a coder, managing PRs and cross-bot communication.

**Source credibility:** Active repository with specific, practical tool-chain integration instructions.

**Recency:** Highly relevant to modern agentic workflows and Claude Code's ability to interact with development lifecycles.

**Source:** [mshogin/archlint/CLAUDE.md](https://github.com/mshogin/archlint/blob/47b46954dcdf14f8ed8edc897410890f9c7c3686/CLAUDE.md) · 23★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# archlint - Claude Code Rules

## Communication

- Main bot-to-bot channel: [Issue #3](https://github.com/mshogin/archlint/issues/3)
- Always ping issue #3 when you need action from another contributor
- Use prefixes: `[archi]`, `[kostyaai]`, or `[your_name]`
- Every message should end with a concrete action request

## Pull Requests

- Review ALL open PRs - don't wait for someone to ask
- SLA: first review response within 24 hours
- When creating a PR, add a comment to issue #3 asking for review
- When reviewing, check: code correctness, architecture alignment, test coverage
- End review with clear verdict: "merge", "needs fix X", or "discuss"

## Code Conventions

- Language: Go
- Architecture layers: cmd -> cli -> mcp -> analyzer -> model
- Interfaces: max 5 methods, segregated by responsibility
- Fan-out: max 5 dependencies per component
- Tests required for new functionality
- SOLID principles enforced by archlint itself

## Task Management

- See [TASKS.md](TASKS.md) for current work items and status
- Don't block on waiting for merge approvals - work on other tasks in parallel
- Update TASKS.md when task status changes

## Periodic Tasks

- Check all open PRs for pending re
```

</details>
