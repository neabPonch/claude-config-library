---
name: adrian-thurston__colm-suite
source: https://github.com/adrian-thurston/colm-suite/blob/b6a727beb458a06f31d8ce53bd592915bbd98eff/CLAUDE.md
repo: adrian-thurston/colm-suite
kind: claude-md
stars: 222
last_pushed: 2026-06-06T19:53:32Z
license: mit
score: 9
domains: [compiler-construction, systems-programming]
tags: [compilers, build-instructions, tooling]
curated: 2026-06-14
curated_by: config-scout
---

# adrian-thurston/colm-suite — claude-md

**Why it's worth keeping:** Excellent separation of build vs. development commands and a structured 'Important Notes' section that preemptively addresses bootstrapping order.

**Summary:** Provides deep context on the symbiotic relationship between Colm and Ragel, including specific command flags for different backends.

**Source credibility:** High; a well-starred (222) specialized tool with recent activity.

**Recency:** Current; follows the standard CLAUDE.md structure useful for today's AI coding agents.

**Source:** [adrian-thurston/colm-suite/CLAUDE.md](https://github.com/adrian-thurston/colm-suite/blob/b6a727beb458a06f31d8ce53bd592915bbd98eff/CLAUDE.md) · 222★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with
code in this repository.

## Project Overview

This repository contains two closely related projects:

- **Colm** (COmputer Language Machinery): A programming language and compiler
  construction toolkit designed for analysis and transformation of computer
  languages. Written in C/C++, it generates C code that compiles to native
  executables.

- **Ragel**: A state machine compiler that generates executable finite state
  machines from regular expressions and state machine specifications. It targets
  12+ languages: C, C++, D, Java, Ruby, C#, Go, OCaml, Rust, Julia, JavaScript,
  GNU ASM x86-64, and Crack.

Colm bootstraps Ragel -- Ragel's parser is written in Colm (`src/ragel/*.lm`).

## Build Commands

```bash
# Initial setup (only needed once)
./autogen.sh
./configure

# Build the project (both Colm and Ragel)
make

# Run tests
make check

# Install
make install

# Clean build artifacts
make clean
```

## Development Commands

```bash
# Compile a Colm program
colm file.lm

# Compile and run immediately
colm -r file.lm

# Compile only (don't produce binary)
colm -c file.lm

# Generate dot
```

</details>
