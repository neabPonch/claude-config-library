---
name: videojs__v10
source: https://github.com/videojs/v10/blob/47aca0f798b51b98741cf5d63ba8395e8ff0ad3d/CLAUDE.md
repo: videojs/v10
kind: claude-md
stars: 815
last_pushed: 2026-06-17T02:34:29Z
license: other
score: 9
domains: [web-frontend, monorepo]
tags: [monorepo, typescript, pnpm, workflow]
curated: 2026-06-17
curated_by: config-scout
---

# videojs/v10 — claude-md

**Why it's worth keeping:** The dependency hierarchy diagram and the critical warning that type changes require a build (due to project references) are high-value instructions that prevent common developer/AI errors.

**Summary:** Provides deep structural context for a complex monorepo and precise development workflows tailored for AI agents. It includes architectural constraints to maintain code quality across different platforms.

**Source credibility:** High; Video.js is a highly-starred, industry-standard media framework with active maintenance.

**Recency:** Current; explicitly optimizes for Claude Code and modern toolchains like PNPM, Turbo, and Vitest.

**Source:** [videojs/v10/CLAUDE.md](https://github.com/videojs/v10/blob/47aca0f798b51b98741cf5d63ba8395e8ff0ad3d/CLAUDE.md) · 815★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Guidance for **Claude Code** (claude.ai/code) and other AI agents working with this repository.

## Overview

**Video.js 10** is a **Turborepo‑managed monorepo**, organized by runtime and platform.
Refer to **[`CONTRIBUTING.md`](./CONTRIBUTING.md)** for setup, development, and lint/test instructions.

## Package Layout

| Package Path            | Purpose                                                             |
| ----------------------- | ------------------------------------------------------------------- |
| `packages/utils`        | Shared utilities (`/dom` subpath for DOM‑specific helpers).         |
| `packages/element`      | Custom element base class for web components.                       |
| `packages/store`        | State management (`/html`, `/react` subpaths for platforms).        |
| `packages/spf`          | Stream Processing Framework (`/dom` and `/playback-engine` subpaths for DOM bindings and the HLS engine). |
| `packages/core`         | Core runtime‑agnostic logic (`/dom` subpath for DOM bindings).      |
| `packages/icons`        | SVG icon library (private, consumed by html and react).             |
| `packages/skins`        | Shared skin CSS
```

</details>
