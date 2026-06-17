---
name: yaml__yamlscript__claude
source: https://github.com/yaml/yamlscript/blob/afd49feb1638b2774fb72687871fe58e63c7c05e/.claude.md
repo: yaml/yamlscript
kind: claude-md
stars: 622
last_pushed: 2026-06-14T18:39:03Z
license: mit
score: 9
domains: [cli-tools, compilers]
tags: [makefile, monorepo, coding-standards]
curated: 2026-06-15
curated_by: config-scout
---

# yaml/yamlscript — claude-md

**Why it's worth keeping:** It features hyper-specific formatting rules like exact line wrapping and step-by-step build/testing flows that enable highly reliable agentic automation.

**Summary:** This config provides strict coding style constraints, detailed GNU Make command sets for a monorepo, and an architectural roadmap of the compilation pipeline.

**Source credibility:** High; comes from a legitimate, active programming language project with significant community interest.

**Recency:** Extremely current given the recent commit history.

**Source:** [yaml/yamlscript/.claude.md](https://github.com/yaml/yamlscript/blob/afd49feb1638b2774fb72687871fe58e63c7c05e/.claude.md) · 622★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with
code in this repository.

## Overview

YAMLScript (YS) is a functional programming language that uses YAML syntax and
compiles to Clojure.
It provides:
- A YAML loader library for 15+ programming languages
- A standalone `ys` command-line tool
- Native shared library `libys.so` for language bindings

## Coding style

* **Wrap lines at exactly 80 characters** - This is strictly enforced
* Use 2 spaces for indentation in most languages
* Use styles already established in the file
* Prefer single quotes over double quotes when possible and appropriate
* In yaml files:
  * Don't over-indent sequences in block mappings
  * Don't quote scalar values that don't need to be quoted
* Use `ReadMe.md`, not `README.md`
* For markdown files:
  * **Start each sentence on a new line**
  * **Wrap lines at exactly 80 characters** - count carefully
  * Put 2 blank lines before a section heading

## Common Development Commands

GNU Make is used for all dev tasks.
Almost every directory has a Makefile, and they use the `common/*.mk` files
for shared logic.
They also automatically install the https://github.com/ma
```

</details>
