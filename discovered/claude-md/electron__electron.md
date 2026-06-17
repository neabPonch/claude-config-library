---
name: electron__electron
source: https://github.com/electron/electron/blob/16d0cafbfa5a7084139557c6b28b85320213af6a/CLAUDE.md
repo: electron/electron
kind: claude-md
stars: 121634
last_pushed: 2026-06-14T14:20:48Z
license: mit
score: 10
domains: [cli-tools, build-systems, desktop-apps]
tags: [workflow-automation, patch-management, command-reference]
curated: 2026-06-15
curated_by: config-scout
---

# electron/electron — claude-md

**Why it's worth keeping:** Features high-value 'Never' rules (e.g., banning `npx`), provides dense command tables for internal CLI tools, and includes complex recovery procedures for CI/patch conflicts.

**Summary:** Provides deep technical context on custom build tools, patch management workflows, and strict execution rules.

**Source credibility:** Extremely high; sourced from one of the most significant cross-platform desktop frameworks in existence.

**Recency:** Very current, referencing modern tooling like oxlint and advanced GitHub CLI workflows.

**Source:** [electron/electron/CLAUDE.md](https://github.com/electron/electron/blob/16d0cafbfa5a7084139557c6b28b85320213af6a/CLAUDE.md) · 121634★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Electron Development Guide

## Running node_modules binaries

**Never use `npx`.** It is considered dangerous because it can silently fetch and execute arbitrary packages from the registry. Always run binaries through one of these safer mechanisms instead:

1. **Preferred** — spawn the executable directly from `node_modules/.bin/<tool>` (or the platform equivalent on Windows). This is what `script/lint.js` does for `oxlint`.
2. **Acceptable** — invoke via `yarn <tool>` or `yarn run <tool>`, which resolves to the locally installed version without the registry fallback that `npx` performs.

This rule applies to shell commands you run yourself and to any scripts you author or modify in this repo.

## Project Overview

Electron is a framework for building cross-platform desktop applications using web technologies. It embeds Chromium for rendering and Node.js for backend functionality.

## Directory Structure

```text
electron/                 # This repo (run `e` commands here)
├── shell/               # Core C++ application code
│   ├── browser/         # Main process implementation (107+ API modules)
│   ├── renderer/        # Renderer process code
│   ├── common/          # Shared
```

</details>
