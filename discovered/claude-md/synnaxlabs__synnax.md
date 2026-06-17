---
name: synnaxlabs__synnax
source: https://github.com/synnaxlabs/synnax/blob/d68c4490438632e1ce1a6a583cd8f7dd92988d6c/CLAUDE.md
repo: synnaxlabs/synnax
kind: claude-md
stars: 120
last_pushed: 2026-06-14T23:03:16Z
license: other
score: 10
domains: [monorepo, hardware-software, devops]
tags: [multi-language, git-workflow, instruction-heavy]
curated: 2026-06-15
curated_by: config-scout
---

# synnaxlabs/synnax — claude-md

**Why it's worth keeping:** It provides concrete CLI commands for diverse languages and uses 'hard rules' to prevent LLM behaviors like adding co-author footers or incorrect PR metadata.

**Summary:** A high-fidelity monorepo guide that integrates language-specific toolchains with strict organizational development workflows.

**Source credibility:** High; part of an active, specialized hardware observability platform (synnax).

**Recency:** Very current; specifically addresses modern Claude Code behaviors like git authorship attribution.

**Source:** [synnaxlabs/synnax/CLAUDE.md](https://github.com/synnaxlabs/synnax/blob/d68c4490438632e1ce1a6a583cd8f7dd92988d6c/CLAUDE.md) · 120★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in
this repository.

## Documentation Index

- **Architecture**: See @docs/claude/architecture.md for system design and data flows
- **Testing**: See @docs/claude/testing.md for cross-language testing guide
- **TypeScript**: See @docs/claude/toolchains/typescript.md for TS/JS development
- **Go**: See @docs/claude/toolchains/go.md for Go development
- **Python**: See @docs/claude/toolchains/python.md for Python development
- **C++**: See @docs/claude/toolchains/cpp.md for C++ development
- **Console**: See @docs/claude/components/console.md for Console application details
- **Driver**: See @docs/claude/components/driver.md for hardware driver development

## Quick Start

### Project Structure

Synnax is a **horizontally-scalable observability and control platform** for hardware
telemetry systems. The monorepo includes:

- **TypeScript**: Console (Tauri app), Pluto (viz library), Client, Drift (multi-window
  state)
- **Go**: Server, Cesium (time-series DB), Aspen (distributed KV), Arc (language
  compiler)
- **Python**: Client library, integration test framework
- **C++**: Driver system
```

</details>
