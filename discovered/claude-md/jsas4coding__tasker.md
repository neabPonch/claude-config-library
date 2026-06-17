---
name: jsas4coding__tasker
source: https://github.com/jsas4coding/tasker/blob/ada6616fff11bc56ae1c24b86ea48c0908298cf1/CLAUDE.md
repo: jsas4coding/tasker
kind: claude-md
stars: 0
last_pushed: 2026-02-26T10:54:08Z
license: mit
score: 8
domains: [cli-tools, go]
tags: [golang, architecture, workflow]
curated: 2026-06-15
curated_by: config-scout
---

# jsas4coding/tasker — claude-md

**Why it's worth keeping:** It captures critical 'tribal knowledge' like specific schema update workflows and task naming patterns that are essential for preventing regressions in a complex CLI tool.

**Summary:** A high-density document that maps the directory tree to logical responsibilities and establishes strict procedural rules for schema management.

**Source credibility:** The repository has low social proof (0 stars), but the content reflects highly professional Go project organization.

**Recency:** Current; follows modern Go standards and architectural patterns.

**Source:** [jsas4coding/tasker/CLAUDE.md](https://github.com/jsas4coding/tasker/blob/ada6616fff11bc56ae1c24b86ea48c0908298cf1/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Tasker - CLAUDE.md

## Project Overview

Tasker is a Go CLI tool that reads structured configuration (`.tasker/config.yml` + `.tasker/tasks/*.yml`) and bundles into a single `Taskfile.yml` and `Makefile`.

## Architecture

```
tasker/
├── cmd/tasker/
│   └── main.go                      # Entry point
├── internal/
│   ├── cmd/                         # CLI commands (cobra)
│   │   ├── root.go                  # Root command, default → generate
│   │   ├── generate.go              # Bundle and output files
│   │   ├── init.go                  # Scaffold new project
│   │   ├── validate.go              # Config validation
│   │   ├── list.go                  # Structured help/list
│   │   ├── completion.go            # Shell completions for tasker CLI
│   │   └── version.go              # Version display (ldflags)
│   ├── config/                      # Configuration parsing
│   │   ├── config.go                # Config schema + loading
│   │   ├── group.go                 # Group + task schema, task file loading
│   │   ├── environment.go           # Environment schema
│   │   ├── detect.go                # Package manager detection
│   │   ├── schema.go                # JSON Schem
```

</details>
