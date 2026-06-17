---
name: ChiChou__grapefruit__skill
source: https://github.com/ChiChou/grapefruit/blob/98373c60d005bc320d0d32e523fda11397296efa/skills/igf/SKILL.md
repo: ChiChou/grapefruit
kind: skill
stars: 1332
last_pushed: 2026-05-21T23:08:42Z
license: mit
score: 9
domains: [security, mobile-testing, cli-tools]
tags: [ios, android, security-research, instrumentation]
curated: 2026-06-15
curated_by: config-scout
---

# ChiChou/grapefruit — skill

**Why it's worth keeping:** It clearly defines the mandatory distinction between stateless commands and stateful agent sessions requiring specific session options, preventing execution errors. The logical grouping of command namespaces makes it highly effective for LLM planning.

**Summary:** Provides comprehensive command documentation for the Grapefruit mobile security instrumentation server, covering device management, file system access, and platform-specific (iOS/Android) analysis.

**Source credibility:** High; based on a popular open-source mobile security project with over 1.3k stars.

**Recency:** 

**Source:** [ChiChou/grapefruit/skills/igf/SKILL.md](https://github.com/ChiChou/grapefruit/blob/98373c60d005bc320d0d32e523fda11397296efa/skills/igf/SKILL.md) · 1332★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: igf
description: >-
  CLI interface for igf (Grapefruit) dynamic instrumentation server.
  Use to enumerate Frida devices, list apps, run hooks, query logs,
  access device file systems, inspect classes, dump memory, and
  perform mobile app security analysis.
---

# IGF (Grapefruit) CLI Skill

You are a CLI tool for interacting with the igf (Grapefruit) dynamic instrumentation server. The server runs at `http://localhost:31337` by default (port configurable via `PORT` env or `--port` flag).

## Architecture

IGF has two communication layers:

1. **REST API** (stateless) — HTTP endpoints for device enumeration, history queries, file transfers
2. **Socket.IO RPC** (stateful) — WebSocket session for real-time agent control, requires an active Frida session

RPC calls go through Socket.IO: `emit("rpc", namespace, method, args, callback)`.
The agent organizes methods by namespace (e.g., `fs.ls`, `pins.start`, `classes.list`).

## How to Execute

Use the `igf` CLI directly. All commands follow the pattern:

```
igf <command> [subcommand] [args] [options]
```

### Global Options

- `-H, --host <host>` — Server host (default: localhost)
- `-p, --port <port>` — Server port (defau
```

</details>
