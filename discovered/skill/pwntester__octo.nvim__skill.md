---
name: pwntester__octo.nvim__skill
source: https://github.com/pwntester/octo.nvim/blob/7fed87415c401954f73401bbed0fd736b9611e7c/.agents/skills/execute-lua/SKILL.md
repo: pwntester/octo.nvim
kind: skill
stars: 3306
last_pushed: 2026-06-05T14:49:17Z
license: mit
score: 9
domains: [cli-tools, development-environment]
tags: [lua, neovim, debugging, headless]
curated: 2026-06-15
curated_by: config-scout
---

# pwntester/octo.nvim — skill

**Why it's worth keeping:** The differentiation between execution modes and the proactive path-discovery step provide a superior pattern for agentic environmental debugging.

**Summary:** Provides structured methods to execute Lua code across varying Neovim runtime environments, ranging from isolated plugin tests to full user configurations.

**Source credibility:** High; derived from an extremely popular and actively maintained Neovim plugin (octo.nvim).

**Recency:** Current; utilizes modern headless Neovim execution patterns and Lua best practices.

**Source:** [pwntester/octo.nvim/.agents/skills/execute-lua/SKILL.md](https://github.com/pwntester/octo.nvim/blob/7fed87415c401954f73401bbed0fd736b9611e7c/.agents/skills/execute-lua/SKILL.md) · 3306★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: execute-lua
description: >
  Use this skill when you need to execute, test, or debug Lua code inside Neovim's runtime
  environment without opening the editor UI. Applies when: inspecting plugin modules (e.g.
  `require "octo.gh"`), verifying API behaviour, reproducing bugs, running one-off scripts
  against plugin code, or checking what functions/tables a module exposes.   Supports four
  modes: fully isolated (no config, simulates a fresh install), dependency-controlled (no
  config but explicit runtimepath), full user environment (real init.lua + lazy.nvim),
  and Plenary Busted test runner (relative paths, no filesystem assumptions).
  Prefer this over plain `lua` or `luajit` when the code uses `vim.*` APIs or depends on
  Neovim's plugin runtimepath.
---

When you need to exercise Lua code in the exact Neovim environment that the user has installed, shell out to `nvim` with the `-es` headless flags and pass a temporary Lua script via `-l`.

There are four distinct execution modes depending on the goal.

---

## Finding the key paths

Before running any mode, resolve these paths and store them in shell variables. Run this once to discover them:

```bash
# Neovim confi
```

</details>
