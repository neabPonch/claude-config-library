---
name: formatjs__formatjs
source: https://github.com/formatjs/formatjs/blob/41cd6413e934dd524835d4c217038bffc6c44683/CLAUDE.md
repo: formatjs/formatjs
kind: claude-md
stars: 14719
last_pushed: 2026-06-15T10:56:51Z
license: unknown
score: 9
domains: [monorepo, build-systems, typescript, rust, cli-tools]
tags: [bazel, monorepo, architecture-guardrails, high-signal]
curated: 2026-06-15
curated_by: config-scout
---

# formatjs/formatjs — claude-md

**Why it's worth keeping:** Uses 'negative constraints' (e.g., NEVER run bazel clean) to prevent costly errors and implements a scalable 'Knowledge Base' pointer system instead of bloating the main file.

**Summary:** Provides high-density architectural constraints and build-system guardrails for a complex Bazel/TypeScript/Rust monorepo.

**Source credibility:** Highly credible; based on a high-star, actively maintained enterprise-grade monorepo.

**Recency:** 

**Source:** [formatjs/formatjs/CLAUDE.md](https://github.com/formatjs/formatjs/blob/41cd6413e934dd524835d4c217038bffc6c44683/CLAUDE.md) · 14719★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Instructions for Claude Code

## Knowledge Base

For detailed architecture docs, package dependency hierarchies, CLDR data pipelines, and design decisions, consult @knowledge-base/. Key docs:

- @knowledge-base/001-repo-layout.md — Directory structure, pnpm, linting, CI/CD, common commands
- @knowledge-base/001a-bazel-toolchain.md — Bazel setup, TypeScript/Rust build pipeline, custom macros, tsconfig strategy, composite sub-packages
- @knowledge-base/002-ts-package-dependency-hierarchy.md — 5-layer TypeScript package dependency graph
- @knowledge-base/003-rust-crate-dependency-hierarchy.md — Rust crates, WASM, cross-language connections
- @knowledge-base/004-009 — Per-package design decisions and ECMA-402 conformance details
- @knowledge-base/007a-007k — Individual polyfill CLDR data pipelines
- @knowledge-base/migrations/ — Migration plans (e.g., gazelle migration)

## Critical Rules

### 1. NEVER Run `bazel clean`

- **NEVER** run `bazel clean` or `bazel clean --expunge`
- Destroys build cache, 10+ minute rebuild penalty
- Use specific targets instead: `bazel build //path/to:target`

### 2. Always Use Bazel

This repository uses Bazel as its build system. Never use `npm`, `yarn
```

</details>
