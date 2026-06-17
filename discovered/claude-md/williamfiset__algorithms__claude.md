---
name: williamfiset__algorithms__claude
source: https://github.com/williamfiset/algorithms/blob/4371d09f17a355f2ecaa216111b1c2e546a752c8/.claude.md
repo: williamfiset/algorithms
kind: claude-md
stars: 18637
last_pushed: 2026-04-03T22:50:09Z
license: mit
score: 9
domains: [algorithms, java, build-systems]
tags: [bazel, java, algorithmic-templates]
curated: 2026-06-15
curated_by: config-scout
---

# williamfiset/algorithms — claude-md

**Why it's worth keeping:** It includes exact CLI command patterns for running tests/binaries and a prescriptive step-by-step workflow for extending the codebase.

**Summary:** Defines strict educational coding principles alongside specific Bazel build/test commands and directory mappings.

**Source credibility:** High; the repository is highly starred (18k+) and actively maintained.

**Recency:** Current; reflects modern Java development workflows with Bazel.

**Source:** [williamfiset/algorithms/.claude.md](https://github.com/williamfiset/algorithms/blob/4371d09f17a355f2ecaa216111b1c2e546a752c8/.claude.md) · 18637★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Purpose

This is an **educational algorithms and data structures repository**. The core goal is to provide clear, well-tested, and accessible implementations for learners who may not have deep computer science backgrounds.

**Key Principles:**
- **Every file should teach**, not just implement.
- Implementations should be simple, elegant, and avoid unnecessary complexity (e.g., prefer plain loops over Java Streams).
- Documentation must explain *how* and *why* an algorithm works, including time and space complexity.
- Every algorithm must be accompanied by comprehensive tests that cover edge cases and teach through examples.

## Build System

This project uses **Bazel** as its build system (requires JDK 8+). Dependencies are managed via Maven through `rules_jvm_external` and declared in `MODULE.bazel`.

## Commands

**Run all tests:**
```bash
bazel test //src/test/...
```

**Run tests for a specific package:**
```bash
bazel test //src/test/java/com/williamfiset/algorithms/graphtheory:all
bazel test //src/test/java/com/williamfiset/algorithms/sorting:all
```
```

</details>
