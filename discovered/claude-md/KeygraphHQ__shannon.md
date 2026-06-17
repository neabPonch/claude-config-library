---
name: KeygraphHQ__shannon
source: https://github.com/KeygraphHQ/shannon/blob/3d1a3c75f82d96d0614b74e463d2be101b7804f1/CLAUDE.md
repo: KeygraphHQ/shannon
kind: claude-md
stars: 44592
last_pushed: 2026-06-12T09:27:40Z
license: agpl-3.0
score: 9
domains: [security, cli-tools, agents-ai, devops]
tags: [monorepo, docker, temporal, pentesting]
curated: 2026-06-15
curated_by: config-scout
---

# KeygraphHQ/shannon — claude-md

**Why it's worth keeping:** It provides exhaustive command mapping for different environments (npx vs local) and maps business logic to specific file paths, ensuring the AI understands the system's operational modes.

**Summary:** A comprehensive technical manual detailing dual-mode CLI execution, monorepo architecture, and complex container orchestration.

**Source credibility:** High-authority repository with over 44k stars and very recent maintenance.

**Recency:** Extremely current; reflects modern monorepo and containerized development workflows.

**Source:** [KeygraphHQ/shannon/CLAUDE.md](https://github.com/KeygraphHQ/shannon/blob/3d1a3c75f82d96d0614b74e463d2be101b7804f1/CLAUDE.md) · 44592★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

AI-powered penetration testing agent for defensive security analysis. Automates vulnerability assessment by combining reconnaissance tools with AI-powered code analysis.

## Commands

**Prerequisites:** Docker, AI provider credentials (`.env` for local, `shn setup` or env vars for npx)

### Dual CLI

Shannon supports two CLI modes, auto-detected based on the current working directory:

| | **npx** (`npx @keygraph/shannon`) | **Local** (`./shannon`) |
|---|---|---|
| **Install** | Zero-install via npm | Clone the repo |
| **Image** | Pulled from Docker Hub (`keygraph/shannon:latest`) | Built locally (`shannon-worker`) |
| **State** | `~/.shannon/` | Project directory |
| **Credentials** | `~/.shannon/config.toml` (via `shn setup`) or env vars | `./.env` |
| **Config** | `~/.shannon/config.toml` (via `shn setup`) | N/A |
| **Prompts** | Bundled in Docker image | Mounted from `./apps/worker/prompts/` (live-editable) |

Mode auto-detection: local mode activates when env var `SHANNON_LOCAL=1` is set by the `./shannon` entry point (`apps/cli/src/mode.ts`). Otherwise npx mode.

### npx Quick Start

```bash
# Configure credentials (interactive wizard)
npx @keygraph/shannon set
```

</details>
