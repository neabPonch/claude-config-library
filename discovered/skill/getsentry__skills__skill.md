---
name: getsentry__skills__skill
source: https://github.com/getsentry/skills/blob/b39c7c4b6056f0579b340b7c5c4e811e400368e8/skills/agents-md/SKILL.md
repo: getsentry/skills
kind: skill
stars: 797
last_pushed: 2026-06-12T23:55:03Z
license: apache-2.0
score: 9
domains: [agents-ai, developer-experience]
tags: [markdown, templates, instructions]
curated: 2026-06-15
curated_by: config-scout
---

# getsentry/skills — skill

**Why it's worth keeping:** The emphasis on file-scoped commands (rather than global ones) and the 'no-prose' rule prevents instruction drift and optimizes token usage. The use of structured tables for command/reference lookups is a top-tier technique for agentic clarity.

**Summary:** A highly disciplined protocol for creating minimal, high-signal AGENTS.md/CLAUDE.md files tailored for AI agents. It prioritizes strict structure and exact referencing over verbose prose.

**Source credibility:** High; Sentry is a major engineering organization with an active, high-quality repository.

**Recency:** Extremely current; aligns perfectly with the latest agentic coding workflows and Claude Code patterns.

**Source:** [getsentry/skills/skills/agents-md/SKILL.md](https://github.com/getsentry/skills/blob/b39c7c4b6056f0579b340b7c5c4e811e400368e8/skills/agents-md/SKILL.md) · 797★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: agents-md
description: Creates and maintains concise AGENTS.md and CLAUDE.md project instruction files. Use when asked to create AGENTS.md, update AGENTS.md, maintain agent docs, set up CLAUDE.md, document repository agent conventions, or keep coding-agent instructions minimal and reference-backed.
---

# Maintaining AGENTS.md

Goal: concise, actionable agent instructions. Target under 60 lines; never exceed 100.

## Workflow

1. Inspect before writing:
   - package manager: lock files and manifests
   - commands: `package.json`, `Makefile`, task runners, CI workflows
   - docs/specs/policies: `README.md`, `CONTRIBUTING.md`, `docs/`, `specs/`, `policies/`, `SECURITY.md`, `.github/`
   - conventions: current code patterns, test layout, generated files, legacy areas to avoid
2. Choose scope:
   - root `AGENTS.md`: repo-wide defaults
   - nested `AGENTS.md`: only when a subtree has different commands or rules
   - closest instruction file wins; keep narrower files shorter than root files
3. Write the smallest useful file.
4. Verify exact paths and commands exist.

## File Setup

- Create `AGENTS.md` at the repository root.
- If a Claude-compatible entrypoint is required, sym
```

</details>
