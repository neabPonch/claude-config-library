---
name: koalaman__shellcheck__claude
source: https://github.com/koalaman/shellcheck/blob/9af7ee28ce587baadd950b85dd6826a16b9c068d/.claude/CLAUDE.md
repo: koalaman/shellcheck
kind: claude-md
stars: 39574
last_pushed: 2026-06-11T03:17:10Z
license: gpl-3.0
score: 10
domains: [cli-tools, static-analysis, haskell]
tags: [architecture, build-commands, contribution-guide]
curated: 2026-06-16
curated_by: config-scout
---

# koalaman/shellcheck — claude-md

**Why it's worth keeping:** Uses structured file-to-purpose mappings, defines explicit contribution workflows, and highlights technical pitfalls like AST 'sugar' vs. desugared representations.

**Summary:** Provides a comprehensive guide for building/testing the tool and highly specific protocols for implementing new static analysis checks.

**Source credibility:** Extremely high; ShellCheck is a widely-used, highly-starred industry standard for shell script analysis.

**Recency:** Current; follows the modern CLAUDE.md pattern of providing context-rich instructions for agentic development.

**Source:** [koalaman/shellcheck/.claude/CLAUDE.md](https://github.com/koalaman/shellcheck/blob/9af7ee28ce587baadd950b85dd6826a16b9c068d/.claude/CLAUDE.md) · 39574★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build and test commands

```sh
cabal build                          # compile
cabal test                           # run unit tests (source of truth)
cabal run shellcheck -- file.sh      # run on a file
cabal run shellcheck - <<< 'cmd'     # run on inline input
./quickrun - <<< 'cmd'               # run interpreted (fast, no recompile)
./quicktest                          # run tests interpreted (fast, no recompile)
./nextnumber                         # print next available SC1xxx/SC2xxx/SC3xxx code
```

For interactive development, use `cabal repl` then `:load ShellCheck.Debug`. After editing, reload with `:r` and test with `shellcheckString "your shell code"`.

To inspect the AST without an interactive session:

```sh
cabal run -fdev-mode shellcheck-dev -- ast 'myshellcommand'
```

## Architecture

ShellCheck processes shell scripts in three stages:

1. **Parsing** (`Parser.hs`) — produces an AST plus warnings (SC1xxx). Parser notes (non-fatal) are buffered and discarded if parsing fails; parser problems (fatal) are always emitted.
2. **AST Analysis** (`Analyti
```

</details>
