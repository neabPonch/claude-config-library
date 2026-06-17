---
name: owellandry__runbox__agent-skill
source: https://github.com/owellandry/runbox/blob/f41f5c34fd61405442f89564d5871eceaca87fbf/skills/AGENT_SKILL.md
repo: owellandry/runbox
kind: skill
stars: 1
last_pushed: 2026-05-08T20:08:19Z
license: unknown
score: 8
domains: [agents-ai, cli-tools, webassembly]
tags: [tool-specification, agent-instructions, sandbox]
curated: 2026-06-15
curated_by: config-scout
---

# owellandry/runbox — skill

**Why it's worth keeping:** The documentation uses perfect 'agent-facing' patterns: explicit JSON input/output examples, strict parameter type definitions, and clear descriptions of error states and side effects.

**Summary:** A highly structured technical specification designed to teach an AI agent how to interact with a specialized WASM-based sandbox runtime. It defines tool schemas, execution protocols, and environmental constraints.

**Source credibility:** Low popularity (1 star), but the technical depth suggests a high-quality specialized developer tool.

**Recency:** Very current; updated within the last month using modern Rust standards.

**Source:** [owellandry/runbox/skills/AGENT_SKILL.md](https://github.com/owellandry/runbox/blob/f41f5c34fd61405442f89564d5871eceaca87fbf/skills/AGENT_SKILL.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# RunBox Agent Skill Guide — Complete Reference

> **Version**: 0.3.9 | **Crate**: `runbox` | **Edition**: Rust 2024 | **License**: MIT
>
> This document is the single source of truth for any AI agent integrating with RunBox.
> It covers every API, every command, every runtime, every pattern, and every edge case.

---

## Table of Contents

1. [Architecture Overview](#1-architecture-overview)
2. [Boot Sequence](#2-boot-sequence)
3. [AI Tool Surface — Complete Reference](#3-ai-tool-surface--complete-reference)
4. [RunboxInstance WASM API — All Public Methods](#4-runboxinstance-wasm-api--all-public-methods)
5. [Command Routing & Runtime Detection](#5-command-routing--runtime-detection)
6. [Runtime Reference — npm / pnpm / yarn](#6-runtime-reference--npm--pnpm--yarn)
7. [Runtime Reference — Bun](#7-runtime-reference--bun)
8. [Runtime Reference — Git](#8-runtime-reference--git)
9. [Runtime Reference — Python](#9-runtime-reference--python)
10. [Runtime Reference — Shell Builtins](#10-runtime-reference--shell-builtins)
11. [Virtual Filesystem (VFS)](#11-virtual-filesystem-vfs)
12. [Console System](#12-console-system)
13. [Process Manager](#13-process-manager)
14. [Hot Reload System](#14-
```

</details>
