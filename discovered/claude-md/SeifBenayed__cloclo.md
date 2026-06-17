---
name: SeifBenayed__cloclo
source: https://github.com/SeifBenayed/cloclo/blob/00f51958cc29660490d57ca5e9bb71e795b64096/CLAUDE.md
repo: SeifBenayed/cloclo
kind: claude-md
stars: 114
last_pushed: 2026-04-05T20:03:07Z
license: mit
score: 10
domains: [cli-tools, agents-ai, nodejs]
tags: [architecture, build-system, testing-guide, agent-protocol]
curated: 2026-06-15
curated_by: config-scout
---

# SeifBenayed/cloclo — claude-md

**Why it's worth keeping:** It includes crucial technical gotchas (like the `extractBlock` limitation) and clearly maps the dependency graph to prevent architectural mistakes. The documentation of the AICL protocol and memory management ensures any agent understands the internal state-machine logic.

**Summary:** A highly technical guide that defines the 'laws of physics' for a complex build system and multi-agent runtime. It explicitly prevents common errors like editing build outputs and provides specific edge cases for testing.

**Source credibility:** High; it's a detailed, specialized SDK with active development/recent pushes.

**Recency:** Very current, with activity within the last two months.

**Source:** [SeifBenayed/cloclo/CLAUDE.md](https://github.com/SeifBenayed/cloclo/blob/00f51958cc29660490d57ca5e9bb71e795b64096/CLAUDE.md) · 114★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# cloclo (claude-native) — Project Conventions

## Architecture

**CRITICAL: `claude-native.mjs` is a BUILD OUTPUT. NEVER edit it directly.**
All source code lives in `src/` (21 modules). Edit there, then run `node build.mjs` to regenerate `claude-native.mjs`. Any direct edit to `claude-native.mjs` will be lost on next build.

Source modules in `src/` (dependency order):
`utils.mjs` → `config.mjs` → `providers.mjs` → `auth.mjs` → `security-rules.mjs` → `security.mjs` → `browser.mjs` → `tools.mjs` → `lsp.mjs` → `auto-memory.mjs` → `memory-metrics.mjs` → `memory-dream.mjs` → `audit.mjs` → `teams.mjs` → `sandbox.mjs` → `context-refs.mjs` → `smart-routing.mjs` → `skill-metrics.mjs` (optional) → `agent-metrics.mjs` (optional) → `aicl.mjs` (optional) → `cron.mjs` → `engine.mjs` → `session.mjs` → `index.mjs`

Ink UI in `ink-ui.mjs` (runtime deps: `ink`, `ink-select-input`, `ink-text-input`, `react`). NDJSON bridge in `claude-tool-loop.js` (~943 lines, supports `stream` and `mcp` modes). `gstack/` is a vendored skill/tool framework sub-project.

npm package: `cloclo` (v1.0.1). Binary: `cloclo`. Shipped files: `claude-native.mjs`, `ink-ui.mjs`, `README.md`, `ROADMAP.md`.

## Testing & Build
```

</details>
