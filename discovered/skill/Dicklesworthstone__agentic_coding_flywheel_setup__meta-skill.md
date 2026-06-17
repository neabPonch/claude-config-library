---
name: Dicklesworthstone__agentic_coding_flywheel_setup__meta-skill
source: https://github.com/Dicklesworthstone/agentic_coding_flywheel_setup/blob/d39a62ef5adc825941b1c98fa89753db9af8e54a/docs/tools/meta_skill.md
repo: Dicklesworthstone/agentic_coding_flywheel_setup
kind: skill
stars: 1509
last_pushed: 2026-06-13T04:34:18Z
license: other
score: 9
domains: [cli-tools, agents-ai, knowledge-management]
tags: [skill-management, semantic-search, orchestration]
curated: 2026-06-14
curated_by: config-scout
---

# Dicklesworthstone/agentic_coding_flywheel_setup — skill

**Why it's worth keeping:** Provides a scalable architecture for prompt engineering by treating skills as searchable knowledge artifacts rather than static context snippets.

**Summary:** A CLI-driven management system designed to organize, index, and retrieve specialized agent skills using hybrid semantic/lexical search.

**Source credibility:** High; highly starred repository with very recent activity.

**Recency:** Highly current and specifically optimized for modern agentic coding workflows.

**Source:** [Dicklesworthstone/agentic_coding_flywheel_setup/docs/tools/meta_skill.md](https://github.com/Dicklesworthstone/agentic_coding_flywheel_setup/blob/d39a62ef5adc825941b1c98fa89753db9af8e54a/docs/tools/meta_skill.md) · 1509★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# meta_skill (ms)

Local-first knowledge management with hybrid semantic search for AI coding agents.

## What It Does

`ms` (meta_skill) provides:
- Skill file management and organization
- Hybrid search (semantic + lexical) over skill content
- Doctor diagnostics for health checks
- Integration with AI agent workflows

Skills are reusable prompts, instructions, and knowledge that agents can invoke during coding sessions.

## Installation Verification

```bash
# Check ms is installed
ms --version

# Run health diagnostics
ms doctor --json
```

Expected: version number and JSON diagnostic report.

## Basic Usage

### List Skills

```bash
# List all available skills
ms list

# List with details
ms list --verbose
```

### Search Skills

```bash
# Semantic search for relevant skills
ms search "git commit workflow"

# Lexical search
ms search "docker" --mode lexical
```

### Show Skill Details

```bash
# Show a specific skill
ms show skill-name

# Show skill content
ms cat skill-name
```

### Health Check

```bash
# Run diagnostics
ms doctor

# JSON output for automation
ms doctor --json
```

## Common Workflows

### Finding Relevant Skills

When starting a task, search for existing sk
```

</details>
