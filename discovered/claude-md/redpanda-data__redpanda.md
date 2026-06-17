---
name: redpanda-data__redpanda
source: https://github.com/redpanda-data/redpanda/blob/61db5552f8e38bfb3e6afc7d56a8ff9cf45c3e09/CLAUDE.md
repo: redpanda-data/redpanda
kind: claude-md
stars: 12204
last_pushed: 2026-06-13T21:22:53Z
license: unknown
score: 9
domains: [systems-programming, backend, high-performance]
tags: [cpp, bazel, async, performance]
curated: 2026-06-15
curated_by: config-scout
---

# redpanda-data/redpanda — claude-md

**Why it's worth keeping:** It features critical 'Do/Don't' coding guidelines that prevent subtle bugs (e.g., memory issues with lambda coroutines) and performance pitfalls related to container usage.

**Summary:** Provides highly detailed build/test instructions for a complex Bazel-based C++ project and includes specific architectural constraints.

**Source credibility:** High; Redpanda is a significant, well-maintained open-source streaming platform.

**Recency:** Current; includes modern C++23 standards and contemporary Bazel/Bazelisk workflows.

**Source:** [redpanda-data/redpanda/CLAUDE.md](https://github.com/redpanda-data/redpanda/blob/61db5552f8e38bfb3e6afc7d56a8ff9cf45c3e09/CLAUDE.md) · 12204★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Copilot Coding Agent Onboarding Guide for `redpanda-data/redpanda`

## High-Level Overview

**What is Redpanda?**

Redpanda is a high-performance, Apache Kafka®-compatible streaming data platform. It is written primarily in C++ for the core, with Go for CLI tooling (`rpk`), and some Python for auxiliary scripts and tests. Redpanda is designed to be lightweight, fast, and simple to operate, omitting ZooKeeper and the JVM.

It uses extensively the thread-per-core model and asynchronous (coroutines, futures) programming model.

**Repository Characteristics:**
- **Large multi-language codebase:** C++ (core), Go (CLI/tools), Python (testing/scripts), Bash and Bazel for builds.
- **Build System:** Bazel (with Bazelisk) for core.
- **Target Platforms:** Linux (primary), some support for macOS and Windows.
- **Key Directories:**
  - `src/v/`: Core C++ source code
  - `src/go/`: Go CLI and tools
  - `bazel/`, `BUILD`, `MODULE.bazel`: Bazel scripts and definitions
  - `tools/`: Development and helper scripts
  - `tests/`: Test suites
  - `conf/`: Configuration files
  - `proto/`: Protobuf definitions for Redpanda services and APIs
  - `.github/`, `.buildkite/`: CI/workflow automation
- **D
```

</details>
