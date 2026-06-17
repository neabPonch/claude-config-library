---
name: yukimemi__dvpm
source: https://github.com/yukimemi/dvpm/blob/174c3f3825d8e36781863783da047f224cdb9e59/CLAUDE.md
repo: yukimemi/dvpm
kind: claude-md
stars: 24
last_pushed: 2026-06-11T02:55:04Z
license: mit
score: 9
domains: [cli-tools, editor-extensions]
tags: [architecture, workflow, typescript, deno]
curated: 2026-06-15
curated_by: config-scout
---

# yukimemi/dvpm — claude-md

**Why it's worth keeping:** The inclusion of the 'Lifecycle' sequence and specific implementation details for concurrency/mapping is highly transferable. It avoids fluff by focusing on how data and control flows through the system.

**Summary:** Provides deep architectural context including a structured lifecycle flow and technical explanations of complex logic like proxy-based lazy loading.

**Source credibility:** High; the repository is actively maintained with very recent updates.

**Recency:** Highly current, specifically optimized for Claude Code instructions.

**Source:** [yukimemi/dvpm/CLAUDE.md](https://github.com/yukimemi/dvpm/blob/174c3f3825d8e36781863783da047f224cdb9e59/CLAUDE.md) · 24★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this
repository.

## What this project is

`dvpm` is a Vim/Neovim plugin manager built on
[denops.vim](https://github.com/vim-denops/denops.vim). It runs as a Deno TypeScript process that
communicates with Vim/Neovim over an RPC bridge. Users write their entire Vim configuration in
TypeScript (`main.ts`), calling dvpm APIs to declare plugins and hooks. dvpm handles installation,
lazy loading, and lifecycle hooks.

## Pull requests

Write PR titles and bodies in English.

## Commands

```sh
deno task check    # type-check all source files
deno task lint     # lint
deno task fmt      # format (--check to verify only)
deno task test     # run tests (clones denops.vim into .test_cache/ if needed)
deno task ci       # check + lint + fmt --check + publish dry-run + test
```

Run a specific test file:

```sh
deno run -A scripts/test_runner.ts tests/lazy_keys_test.ts
```

On this machine, Vim is not available locally — only Neovim tests run. Set
`DENOPS_TEST_VIM_EXECUTABLE=""` to suppress vim-related spawn errors when running tests manually.

## Release process (from GEMINI.md)

1. `deno task
```

</details>
