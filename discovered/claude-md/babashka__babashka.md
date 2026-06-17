---
name: babashka__babashka
source: https://github.com/babashka/babashka/blob/7376bedf59f8820333251b45729eb14c3aa7dee3/CLAUDE.md
repo: babashka/babashka
kind: claude-md
stars: 4538
last_pushed: 2026-06-15T13:32:58Z
license: epl-1.0
score: 9
domains: [cli-tools, language-runtime, compilers]
tags: [clojure, graalvm, native-builds, scripting]
curated: 2026-06-15
curated_by: config-scout
---

# babashka/babashka — claude-md

**Why it's worth keeping:** Excellent documentation of environment-variable-driven features and specific workflows for extending the system via Java classes. It provides clear distinctions between JVM and native execution modes which is critical for this project's correctness.

**Summary:** A comprehensive guide for managing a complex build process involving GraalVM native compilation and conditional feature sets.

**Source credibility:** High; Babashka is a highly-starred, industry-standard Clojure tool with active maintenance.

**Recency:** Current; provides specific tool usage instructions that are highly relevant to modern CLI development workflows.

**Source:** [babashka/babashka/CLAUDE.md](https://github.com/babashka/babashka/blob/7376bedf59f8820333251b45729eb14c3aa7dee3/CLAUDE.md) · 4538★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Babashka is a native Clojure interpreter for scripting with fast startup time. It uses GraalVM to compile to a native binary, designed for scripting tasks where you'd normally use bash but want Clojure's power.

## Build Commands

```bash
# Build uberjar (required before native compilation)
script/uberjar

# Compile to native binary (requires GraalVM, set GRAALVM_HOME)
script/compile

# Run tests on JVM
script/test

# Run tests against native binary
BABASHKA_TEST_ENV=native script/test

# Run library compatibility tests
script/run_lib_tests

# Windows variants
script\uberjar.bat
script\compile.bat
script\test.bat
```

## Development

```bash
# Start REPL
lein repl

# Start REPL with test profile
lein with-profiles +test repl

# Run specific test namespace
lein test :only babashka.main-test

# Run specific test
lein test :only babashka.main-test/some-test-name
```

## Repository Structure

This repo uses git submodules. Clone with `--recursive` or run `git submodule update --init --recursive`.

**Key source paths:**
- `src/babashka/` - Main babash
```

</details>
