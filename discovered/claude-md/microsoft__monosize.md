---
name: microsoft__monosize
source: https://github.com/microsoft/monosize/blob/53759c0caba849c273a64114babbb1040702dafc/CLAUDE.md
repo: microsoft/monosize
kind: claude-md
stars: 48
last_pushed: 2026-06-15T10:15:52Z
license: mit
score: 9
domains: [cli-tools, monorepo]
tags: [nx, typescript, workflow, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# microsoft/monosize — claude-md

**Why it's worth keeping:** It includes high-density 'Architecture notes' explaining module resolution nuances and explicit instructions for the mandatory 'beachball' change file process.

**Summary:** Detailed guidance for a complex monorepo involving core adapter contracts, package roles, and strict versioning workflows.

**Source credibility:** High; maintained by Microsoft with clear tooling documentation.

**Recency:** Current, utilizing modern ESM (.mts), Vitest, and Yarn 4.

**Source:** [microsoft/monosize/CLAUDE.md](https://github.com/microsoft/monosize/blob/53759c0caba849c273a64114babbb1040702dafc/CLAUDE.md) · 48★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository overview

`monosize` is a CLI tool that measures bundle sizes for packages and monorepos and compares them against a stored baseline (typically `main`). This repo is itself a Yarn 4 + Nx monorepo of the CLI plus first-party adapter packages.

The `packages/` directory has three roles:

- `monosize` — the CLI (commands: `measure`, `compare-reports`, `upload-report`). Defines the `BundlerAdapter` and `StorageAdapter` contracts in `packages/monosize/src/types.mts`.
- `monosize-bundler-*` (webpack, rspack, vite) — implement `BundlerAdapter`. Each exposes a factory that takes a config-enhancer callback and returns `{ buildFixture, buildFixtures, name }`. `buildFixture` runs one fixture through the bundler; `buildFixtures` runs many in a single pass (multi-entry) and is what the CLI uses in default `--build-mode=batch`. Vite is the exception: its `buildFixtures` is a sequential loop because rollup's es-lib mode doesn't natively emit multiple self-contained bundles in one pass.
- `monosize-storage-*` (git, upstash) — implement `StorageAdapter` (`getRemoteRepor
```

</details>
