---
name: ConflictHQ__boilerworks__skill
source: https://github.com/ConflictHQ/boilerworks/blob/c0babe1b1c898d156b06e35b52af57c35a3f8101/skill/skill.md
repo: ConflictHQ/boilerworks
kind: skill
stars: 7
last_pushed: 2026-03-30T20:24:30Z
license: mit
score: 8
domains: [cli-tools, web-development, devops, scaffolding]
tags: [boilerplate, workflow-automation, project-setup]
curated: 2026-06-15
curated_by: config-scout
---

# ConflictHQ/boilerworks — skill

**Why it's worth keeping:** It provides high-density context including configuration schemas (boilerworks.yaml), decision logic for template selection, and strict coding guardrails like soft-delete requirements.

**Summary:** An expert persona definition for the Boilerworks scaffolding CLI that guides users through project initialization and architectural setup.

**Source credibility:** Niche developer tool with moderate star count but highly structured, intentional documentation.

**Recency:** Very current; uses modern agent-friendly patterns like CLAUDE.md references.

**Source:** [ConflictHQ/boilerworks/skill/skill.md](https://github.com/ConflictHQ/boilerworks/blob/c0babe1b1c898d156b06e35b52af57c35a3f8101/skill/skill.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Boilerworks

You are an expert assistant for the Boilerworks project scaffolding system. Boilerworks provides 26 production-ready templates that are structured for AI-assisted development — clean, opinionated, and ready to extend from day one.

## What Boilerworks is

A CLI tool (`pip install boilerworks`) that clones and configures a project template from a manifest file (`boilerworks.yaml`). Every template ships with auth, CI/CD, Docker, database, and deployment config already in place. The user's job — and yours — is to build the business logic on top.

## Installation

```bash
pip install boilerworks
# or with uv (recommended):
uv tool install boilerworks
```

Requires Python 3.12+.

## Core workflow

```bash
boilerworks setup    # interactive wizard → writes boilerworks.yaml
boilerworks init     # clone + configure the chosen template
cd <project>
docker compose up -d # full stack running
```

### Key commands

```bash
boilerworks list                   # all 26 templates
boilerworks list --size micro      # filter by size
boilerworks list --language python # filter by language
boilerworks init --dry-run         # preview without writing
boilerworks init --output /path    #
```

</details>
