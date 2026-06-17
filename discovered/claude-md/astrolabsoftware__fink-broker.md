---
name: astrolabsoftware__fink-broker
source: https://github.com/astrolabsoftware/fink-broker/blob/8aca7beb2bfdc2ff7b4fa7f5c06fb1718ed872bb/CLAUDE.md
repo: astrolabsoftware/fink-broker
kind: claude-md
stars: 85
last_pushed: 2026-06-12T20:33:51Z
license: apache-2.0
score: 7
domains: [data-engineering, devops]
tags: [guardrails, automation, git-hygiene]
curated: 2026-06-14
curated_by: config-scout
---

# astrolabsoftware/fink-broker — claude-md

**Why it's worth keeping:** Uses highly effective negative constraints (preventing unnecessary file/doc creation) and provides a specific pattern for speeding up agent workflows via auto-approved operations.

**Summary:** Establishes strict operational guardrails for file creation and git hygiene while providing an auto-approval whitelist to streamline tool usage.

**Source credibility:** Legitimate specialized scientific software repository with active maintenance.

**Recency:** Current; includes tool-specific syntax compatible with modern Claude Code capabilities.

**Source:** [astrolabsoftware/fink-broker/CLAUDE.md](https://github.com/astrolabsoftware/fink-broker/blob/8aca7beb2bfdc2ff7b4fa7f5c06fb1718ed872bb/CLAUDE.md) · 85★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Instructions for Fink-Broker Project

## Project Context
- Working directory: Same directory as this CLAUDE.md file
- Current branch: Use `git branch --show-current` to determine
- Main branch: `master`
- Git repository: astrolabsoftware/fink-broker

## Development Guidelines
- Help as a devops and development expert
- Never add claude as co-author
- All commit messages, logs and comments are in English
- Do what has been asked; nothing more, nothing less
- NEVER create files unless absolutely necessary for achieving the goal
- ALWAYS prefer editing an existing file to creating a new one
- NEVER proactively create documentation files (*.md) or README files unless explicitly requested

## Auto-approved Operations
The following operations can be performed without user approval:
- `WebFetch(domain:github.com)` - Fetch content from GitHub
- `Read($HOME/src/github.com/k8s-school/home-ci/.github/workflows/**)` - Read workflow files from k8s-school project
- `Read($HOME/src/github.com/astrolabsoftware/fink-broker-images/**)` - Read files from fink-broker-images project
- `Bash(git add:*)` - Run git add commands
- `Bash(git commit:*)` - Run git commit commands
- `Bash(git pus
```

</details>
