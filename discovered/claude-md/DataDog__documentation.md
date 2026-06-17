---
name: DataDog__documentation
source: https://github.com/DataDog/documentation/blob/801e3697e52e19008555a9667859dc1c2bea082c/CLAUDE.md
repo: DataDog/documentation
kind: claude-md
stars: 608
last_pushed: 2026-06-15T03:28:42Z
license: other
score: 9
domains: [documentation, web-development]
tags: [hugo, content-workflow, style-guide]
curated: 2026-06-15
curated_by: config-scout
---

# DataDog/documentation — claude-md

**Why it's worth keeping:** Includes an elite 'Don't use / Use instead' table for consistent prose and provides specific Git/Jira workflow constraints to prevent pipeline failures.

**Summary:** Comprehensive developer experience (DX) guide for a Hugo-based documentation site covering builds, CI/CD constraints, and strict style guidelines.

**Source credibility:** High; produced by a major engineering organization with rigorous documentation standards.

**Recency:** Current; explicitly references Claude Code and modern toolchains.

**Source:** [DataDog/documentation/CLAUDE.md](https://github.com/DataDog/documentation/blob/801e3697e52e19008555a9667859dc1c2bea082c/CLAUDE.md) · 608★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is the Datadog Documentation repository, built using Hugo (static site generator) and published to docs.datadoghq.com. The codebase consists of markdown content, Hugo themes, Node.js build scripts, and Python automation tools.

## Development Commands

### Build and Development
- `yarn start` or `make start` - Full build including external dependencies and run development server
- `yarn run start` - Basic Hugo development server (port 1313)
- `make start-no-pre-build` - Skip external dependencies, build and run
- `make start-preserve-build` - Keep existing build scripts for local testing
- `make start-docker` - Build and run via Docker container

### Build Commands
- `yarn build` or `make build` - Production build
- `yarn run build:hugo` - Run Hugo build only
- `yarn run build:preview` - Build with preview environment
- `make build-cdocs` - Compile .mdoc files to HTML

### Testing and Quality
- `yarn run jest-test` - Run JavaScript tests
- `make clean` - Clean generated files
- `make clean-all` - Clean everything (environment, repos, gene
```

</details>
