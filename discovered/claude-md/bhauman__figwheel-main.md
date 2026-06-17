---
name: bhauman__figwheel-main
source: https://github.com/bhauman/figwheel-main/blob/72e4c96a860a7b02859239abd4419cc68940695a/CLAUDE.md
repo: bhauman/figwheel-main
kind: claude-md
stars: 652
last_pushed: 2026-03-17T03:45:33Z
license: epl-1.0
score: 9
domains: [cli-tools, build-systems]
tags: [architecture-mapping, dependency-management, clojure]
curated: 2026-06-15
curated_by: config-scout
---

# bhauman/figwheel-main — claude-md

**Why it's worth keeping:** The 'Architecture' section maps namespaces to roles rather than just listing files, and the 'Development Notes' include critical technical nuances like reader conditionals and auto-generated files.

**Summary:** Provides an excellent architectural map that links specific namespaces to their functional responsibilities and detailed build system instructions.

**Source credibility:** High; a well-starred (650+) specialized tool with recent maintenance activity.

**Recency:** Current; last pushed 3 months ago and follows modern LLM guidance patterns.

**Source:** [bhauman/figwheel-main/CLAUDE.md](https://github.com/bhauman/figwheel-main/blob/72e4c96a860a7b02859239abd4419cc68940695a/CLAUDE.md) · 652★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Figwheel Main is a ClojureScript tooling library providing hot code reloading and live development. It is part of a multi-repo ecosystem alongside sibling projects in `../figwheel-core/` and `../figwheel-repl/`. All three repos are versioned in lockstep (currently 0.2.21-SNAPSHOT).

## Build System

Dual build system: **Leiningen** (`project.clj`) and **Clojure CLI** (`deps.edn`).

For local development with sibling projects, uncomment the `:local/root` entries in `deps.edn` and comment out the `:mvn/version` entries for `figwheel-core` and `figwheel-repl`.

## Common Commands

```bash
# Run tests
lein test                      # or: make testit (cleans first)

# Install all three projects locally (figwheel-core, figwheel-repl, figwheel-main)
make install

# Clean build artifacts
make clean

# Build the helper app (compiled to helper-resources/)
clojure -A:build-helper

# Build documentation
make docs                      # requires Ruby for kramdown markdown processing

# Format code
clojure -A:cljfmt check src/
clojure -A:cljfmt fix src/

# Dep
```

</details>
