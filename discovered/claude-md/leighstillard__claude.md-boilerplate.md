---
name: leighstillard__claude.md-boilerplate
source: https://github.com/leighstillard/claude.md-boilerplate/blob/bd5473a0414e10fe8b475f76f5ca2289974d9957/CLAUDE.md
repo: leighstillard/claude.md-boilerplate
kind: claude-md
stars: 8
last_pushed: 2026-04-14T21:59:40Z
license: unknown
score: 9
domains: [backend-api, devops, security, agents-ai]
tags: [git-discipline, mcp-safety, knowledge-graphs, production-grade]
curated: 2026-06-17
curated_by: config-scout
---

# leighstillard/claude.md-boilerplate — claude-md

**Why it's worth keeping:** The integration of specific memory retrieval protocols (claude-mem/graphify) and the rigorous MCP safety guardrails are high-level techniques for agentic workflows.

**Summary:** An extremely opinionated engineering standard that integrates strict Git discipline with advanced memory management via knowledge graphs.

**Source credibility:** A specialized boilerplate likely authored by an experienced engineer focusing on production-grade agent behaviors.

**Recency:** Highly current, specifically targeting modern Claude Code toolsets and MCP integrations.

**Source:** [leighstillard/claude.md-boilerplate/CLAUDE.md](https://github.com/leighstillard/claude.md-boilerplate/blob/bd5473a0414e10fe8b475f76f5ca2289974d9957/CLAUDE.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Coding Agent Standards

These rules apply to all coding work across the project. Follow them in every session.

## Commit Discipline

- Atomic commits: one logical change per commit.
- Commit messages: imperative mood, under 72 chars for the subject line. Body explains WHY, not WHAT.
- Always commit and push before marking work as complete. Unpushed work does not count.
- Never force-push to main/master. Feature branches only.
- Never skip pre-commit hooks (`--no-verify`). If a hook fails, fix the issue.

## Branch Naming

- Feature: `feature/<issue-number>-<short-description>`
- Bugfix: `fix/<issue-number>-<short-description>`
- Chore: `chore/<short-description>`
- Always branch from the latest main. Rebase before PR if behind.

## Pull Requests

- Title: short, under 70 characters.
- Body: summary of changes, test plan, and link to the GitHub issue.
- One PR per issue. Do not bundle unrelated changes.
- All CI checks must pass before requesting review.

## Tool Usage

### RTK (Rust Token Killer)

RTK runs transparently via a PreToolUse hook. You do not need to invoke it manually.
If `rtk --version` fails or returns unexpected output, stop and report.

### LSP

Use LSP for code
```

</details>
