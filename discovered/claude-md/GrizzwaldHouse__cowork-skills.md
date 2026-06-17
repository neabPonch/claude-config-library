---
name: GrizzwaldHouse__cowork-skills
source: https://github.com/GrizzwaldHouse/cowork-skills/blob/a2a60a2912e308ab0db330b8c9b892ad1fd47732/CLAUDE.md
repo: GrizzwaldHouse/cowork-skills
kind: claude-md
stars: 4
last_pushed: 2026-06-01T08:55:09Z
license: other
score: 9
domains: [cli-tools, ai-agents, security, software-architecture]
tags: [opinionated, architectural-standards, anti-patterns, canonical-sources]
curated: 2026-06-16
curated_by: config-scout
---

# GrizzwaldHouse/cowork-skills — claude-md

**Why it's worth keeping:** Uses a 'Canonical Agent Sources' section to bind the AI to external truths and provides highly specific anti-patterns to prevent 'quick-and-dirty' code generation.

**Summary:** Establishes an authoritative system of coding standards, architectural patterns, and canonical truth sources to guide AI behavior across multiple projects.

**Source credibility:** High; active repository with recent updates and clearly defined professional standards.

**Recency:** Very current; integrates modern Claude Code session tooling and agentic workflows.

**Source:** [GrizzwaldHouse/cowork-skills/CLAUDE.md](https://github.com/GrizzwaldHouse/cowork-skills/blob/a2a60a2912e308ab0db330b8c9b892ad1fd47732/CLAUDE.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Claude Skills System

## Project Overview

A modular system for creating, managing, and syncing Claude AI skill templates. Includes a file watcher, bidirectional sync engine, GitHub integration, and a themed WPF desktop UI with console fallback.

## Tech Stack

- **Language**: Python 3.10+
- **UI**: WPF (XAML) with console fallback (ANSI colors)
- **Sync**: Git-based with hash change detection
- **Platform**: Windows 11 (primary), cross-platform CLI

## Key Directories

- `scripts/` - Python CLI and sync engine (main.py is the entry point)
- `Example_Skills/` - Pre-built skill definitions (6 categories)
- `Skill_Creator/` - Meta-template for creating new skills
- `cloud/` - Sync registry (main_cloud.json stores metadata/hashes/timestamps)
- `config/` - Configuration (watch_config.json)
- `UI_Templates/` - WPF XAML templates
- `skills/` - Active skill packages (canva-designer, design-system, document-designer, universal-coding-standards, architecture-patterns, dev-workflow, enterprise-secure-ai-engineering, desktop-ui-designer, pyqt6-ui-debugger, python-code-reviewer, vault-analysis, verified-build-gate, ai-agents/agentic-parallel)
- `tasks/` - Reusable task checklists
```

</details>
