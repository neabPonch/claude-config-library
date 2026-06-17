---
name: maximn__coding-interview-questions-scala
source: https://github.com/maximn/coding-interview-questions-scala/blob/1ff5cc56d61cb7a7186d1b629ffd8851386d387b/CLAUDE.md
repo: maximn/coding-interview-questions-scala
kind: claude-md
stars: 26
last_pushed: 2026-04-27T20:44:41Z
license: apache-2.0
score: 8
domains: [algorithms, testing]
tags: [scala, sbt, unit-testing]
curated: 2026-06-16
curated_by: config-scout
---

# maximn/coding-interview-questions-scala — claude-md

**Why it's worth keeping:** Provides granular shell commands for running individual tests and explains how to navigate the project's unique trait-mixing testing pattern.

**Summary:** Defines the SBT build lifecycle, specific test execution patterns, and a trait-based testing architecture.

**Source credibility:** A specialized educational repository with modest star count but highly professional documentation structure.

**Recency:** Highly current; uses Scala 3.3.6 LTS and modern sbt workflows.

**Source:** [maximn/coding-interview-questions-scala/CLAUDE.md](https://github.com/maximn/coding-interview-questions-scala/blob/1ff5cc56d61cb7a7186d1b629ffd8851386d387b/CLAUDE.md) · 26★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Scala coding interview questions repository with solutions and comprehensive tests. The codebase demonstrates various algorithmic approaches including recursive, iterative, and tail-recursive implementations.

## Build System

- **Build Tool**: sbt 1.11.5 (Scala Build Tool)
- **Scala Version**: 3.3.6 LTS
- **Test Framework**: Specs2 4.20.8 with ScalaCheck 1.19.0 for property-based testing

## Common Commands

### Building and Testing
```bash
# Clean build artifacts
sbt clean

# Compile the project
sbt compile

# Run all tests
sbt test

# Run tests with coverage
sbt clean coverage test

# Generate coverage report
sbt coverageReport

# Run continuous testing (watch mode)
sbt ~test
```

### Running Specific Tests
```bash
# Run a specific test class
sbt "testOnly org.questions.FibonacciTest"

# Run tests matching a pattern
sbt "testOnly *Fibonacci*"
```

## Code Architecture

### Package Structure
- `org.questions.fibonacci`: Fibonacci implementations (Recursive, Iterative, TailRecursion)
- `org.questions.arrays`: Array-based algorithms (Tw
```

</details>
