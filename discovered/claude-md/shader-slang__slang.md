---
name: shader-slang__slang
source: https://github.com/shader-slang/slang/blob/7432ffa4ea189571a498d481e82f9d8ce337e20b/CLAUDE.md
repo: shader-slang/slang
kind: claude-md
stars: 5371
last_pushed: 2026-06-15T08:08:10Z
license: other
score: 10
domains: [systems-programming, compiler-engineering, cpp]
tags: [build-optimization, reasoning-frameworks, high-level-logic]
curated: 2026-06-15
curated_by: config-scout
---

# shader-slang/slang — claude-md

**Why it's worth keeping:** The 'Problem-Solving Methodology' section teaches the AI high-level reasoning (fixing root causes vs. symptoms), while the build redirection tip is a brilliant optimization for LLM token usage.

**Summary:** Provides specialized build commands with token-saving build strategies and a rigorous 'principled path' engineering philosophy.

**Source credibility:** High; part of a popular, highly-active repository (5k+ stars) used in GPU programming.

**Recency:** Extremely current; updated within the last month and specifically optimized for LLM interaction.

**Source:** [shader-slang/slang/CLAUDE.md](https://github.com/shader-slang/slang/blob/7432ffa4ea189571a498d481e82f9d8ce337e20b/CLAUDE.md) · 5371★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

**Repository**: shader-slang/slang - A shading language for GPU programming
**Primary Language**: C++ with custom Slang language
**MCP Tool Available**: `mcp__deepwiki__ask_question` with repoName: "shader-slang/slang"

Reference other instruction files as well:

- @.github/copilot-instructions.md (shares formatting/testing/debugging info; this CLAUDE.md is the canonical source)

User-specific instructions for Slang (optional, may not exist):

- @~/.claude/slang-instructions.md

## Build System and Common Commands

### Building the Project

If you are running in a Windows sandbox, run extras\win-sandbox-build.bat to produce a build in
debug configuration. This script discovers Visual Studio, runs vcvarsall.bat, configures with the
`vs2022-dev` preset, prefers locally cached dependencies instead of fetching them over the network,
and defaults to building `slangc`, `slang-test`, and `slangi`. Pass extra target names if you need
something other than that default target set.

On non-Windows platforms (Linux/macOS), run cmake directly to build:

```bash
# Configure with d
```

</details>
