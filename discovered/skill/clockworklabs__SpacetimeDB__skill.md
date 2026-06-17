---
name: clockworklabs__SpacetimeDB__skill
source: https://github.com/clockworklabs/SpacetimeDB/blob/b0a8070c959050991453a7fa08e6139c962f9c88/skills/cli/SKILL.md
repo: clockworklabs/SpacetimeDB
kind: skill
stars: 24724
last_pushed: 2026-06-15T07:55:37Z
license: other
score: 8
domains: [cli-tools, backend-database, devops]
tags: [spacetime-db, cli-reference, tooling]
curated: 2026-06-15
curated_by: config-scout
---

# clockworklabs/SpacetimeDB — skill

**Why it's worth keeping:** Uses high-intent 'triggers' to signal tool relevance and organizes command syntax into logical workflows with a dedicated troubleshooting section for error recovery.

**Summary:** A highly structured CLI reference for SpacetimeDB covering project lifecycle, database interaction, and server management.

**Source credibility:** High; sourced from a widely used repository with 24k+ stars.

**Recency:** Current; utilizes modern agentic metadata like triggers and glob patterns.

**Source:** [clockworklabs/SpacetimeDB/skills/cli/SKILL.md](https://github.com/clockworklabs/SpacetimeDB/blob/b0a8070c959050991453a7fa08e6139c962f9c88/skills/cli/SKILL.md) · 24724★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cli
description: SpacetimeDB CLI reference for initializing projects, building modules, publishing databases, querying data, and managing servers
license: Apache-2.0
metadata:
  author: clockworklabs
  version: "2.0"
  role: shared
  language: all
  cursor_globs: "**/*"
  cursor_always_apply: false
triggers:
  - spacetime init
  - spacetime build
  - spacetime publish
  - spacetime dev
  - spacetime sql
  - spacetime call
  - spacetime logs
  - spacetime server
  - spacetime login
  - spacetime generate
  - how do I use the CLI
  - CLI command
---

# SpacetimeDB CLI

Use this skill when the user needs help with the `spacetime` CLI tool - initializing projects, building modules, publishing databases, querying data, managing servers, or troubleshooting CLI issues.

## Quick Reference

### Project Initialization & Development

```bash
# Initialize new project
spacetime init my-project --lang rust|csharp|typescript|cpp
spacetime init my-project --template <template-id>

# Build module
spacetime build                    # release build
spacetime build --debug            # faster iteration, slower runtime

# Dev mode (auto-rebuild, auto-publish, generates bindings)
spacetime de
```

</details>
