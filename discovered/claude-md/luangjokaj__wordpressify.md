---
name: luangjokaj__wordpressify
source: https://github.com/luangjokaj/wordpressify/blob/df91d7e2d2ef991d6818c3ea8ce3d5572b500a56/CLAUDE.md
repo: luangjokaj/wordpressify
kind: claude-md
stars: 1642
last_pushed: 2026-05-26T00:07:03Z
license: mit
score: 9
domains: [web-development, devops, wordpress]
tags: [docker, workflow-automation, gulp, build-pipeline]
curated: 2026-06-14
curated_by: config-scout
---

# luangjokaj/wordpressify — claude-md

**Why it's worth keeping:** It explicitly defines command execution contexts (local vs. inside Docker) and documents critical technical nuances like the use of file polling for Docker volume compatibility.

**Summary:** A highly detailed blueprint for a Docker-based WordPress development workflow that maps out complex build pipelines and service dependencies.

**Source credibility:** High; the project is well-established with over 1600 stars on GitHub.

**Recency:** Current; provides all the specific architectural context required by modern AI coding agents.

**Source:** [luangjokaj/wordpressify/CLAUDE.md](https://github.com/luangjokaj/wordpressify/blob/df91d7e2d2ef991d6818c3ea8ce3d5572b500a56/CLAUDE.md) · 1642★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

WordPressify is a Docker-based WordPress block theme development workflow. It provides an automated build pipeline (Gulp + PostCSS + Babel), live reloading via BrowserSync, and a production export that generates a distributable theme zip.

The project also ships a CLI installer (`npx wordpressify`) that scaffolds new projects by downloading files from GitHub.

## Commands

All npm scripts run from the `installer/package.json` context (the working directory after install). The root `package.json` is only for the CLI installer published to npm.

```bash
# Development
npm start              # docker compose up (starts all services)
npm run build          # docker compose build (rebuild images)
npm run delete         # docker compose down -v (remove containers + volumes)
npm run rebuild        # full teardown + rebuild

# Inside Docker (these run via gulp in the nodejs container)
npm run dev            # gulp dev - watch, compile, BrowserSync on port 3010
npm run prod           # gulp prod - minified build to ./dist/
npm run backup         # gulp bac
```

</details>
