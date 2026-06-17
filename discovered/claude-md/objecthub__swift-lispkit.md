---
name: objecthub__swift-lispkit
source: https://github.com/objecthub/swift-lispkit/blob/cdf88b8144e54333364e096e3de5ec03d4f05830/CLAUDE.md
repo: objecthub/swift-lispkit
kind: claude-md
stars: 426
last_pushed: 2026-06-05T23:38:48Z
license: apache-2.0
score: 9
domains: [systems-programming, language-implementations]
tags: [swift, lisp, compiler-design]
curated: 2026-06-15
curated_by: config-scout
---

# objecthub/swift-lispkit — claude-md

**Why it's worth keeping:** The detailed subsystem breakdowns allow the AI to understand relationships between files rather than just seeing a directory tree; explicit execution flags reduce trial-and-error when running the REPL or programs.

**Summary:** Provides deep architectural context by mapping high-level logic to specific source files and offers exhaustive build/run commands for various environments.

**Source credibility:** High; highly regarded Swift project with significant star count and recent maintenance.

**Recency:** Current; utilizes modern Swift 6 standards and contemporary build workflows.

**Source:** [objecthub/swift-lispkit/CLAUDE.md](https://github.com/objecthub/swift-lispkit/blob/cdf88b8144e54333364e096e3de5ec03d4f05830/CLAUDE.md) · 426★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

LispKit is a framework for building Lisp-based extension and scripting languages for macOS and iOS applications. It implements a core language based on the R7RS (small) Scheme standard, fully written in Swift 6. The framework consists of a compiler, virtual machine, garbage collector, and extensive library system.

## Build Commands

### Using Swift Package Manager

**Build debug binary:**
```bash
swift build -Xswiftc "-D" -Xswiftc "SPM"
```

**Build release binary:**
```bash
swift build -c release -Xswiftc "-D" -Xswiftc "SPM"
```

**Run REPL (debug):**
```bash
.build/debug/LispKitRepl -r Sources/LispKit/Resources -d LispKit
```

**Run REPL (release):**
```bash
.build/release/LispKitRepl -r Sources/LispKit/Resources -d LispKit
```

**Execute a Scheme program:**
```bash
.build/debug/LispKitRepl -r Sources/LispKit/Resources -d LispKit path/to/program.scm
```

### Using Makefile

**Build and run debug REPL:**
```bash
make run
```

**Build and run release REPL:**
```bash
make repl
```

**Execute a specific program:**
```bash
make run program=path/to/
```

</details>
