---
name: wasp-lang__wasp
source: https://github.com/wasp-lang/wasp/blob/ea377dac865d368769858a63406170226e4a505f/CLAUDE.md
repo: wasp-lang/wasp
kind: claude-md
stars: 18400
last_pushed: 2026-06-16T15:42:59Z
license: mit
score: 8
domains: [cli-tools, fullstack-framework, compiler-dev]
tags: [monorepo, haskell, typescript, build-system]
curated: 2026-06-16
curated_by: config-scout
---

# wasp-lang/wasp — claude-md

**Why it's worth keeping:** Uses explicit 'Important Rules' to prevent breaking E2E snapshots/docs and maps exact CLI commands for toolchain management.

**Summary:** Provides high-density context including repository structure, multi-phase build processes, and strict technical constraints.

**Source credibility:** High; Wasp is a highly-starred (18k+) and actively maintained full-stack framework.

**Recency:** Extremely current; reflects active development as of this month.

**Source:** [wasp-lang/wasp/CLAUDE.md](https://github.com/wasp-lang/wasp/blob/ea377dac865d368769858a63406170226e4a505f/CLAUDE.md) · 18400★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Wasp Monorepo

Wasp is a full-stack web framework that compiles `.wasp` configuration files into React + Node.js applications. The compiler is written in Haskell.

## Repository Structure

- `waspc/` — Haskell compiler, CLI, and LSP server (the core of Wasp)
  - `src/` — Main compiler library (Analyzer, Generator, AppSpec, Psl)
  - `cli/src/` — CLI commands (start, build, new, deploy, etc.)
  - `waspls/` — Language Server Protocol implementation
  - `data/packages/` — TypeScript packages called by the CLI when compiling projects as FFI
  - `data/Generator/libs/` — TypeScript libraries embedded into generated project code
  - `data/Generator/templates/` — Mustache templates for code generation
  - `e2e-tests/` — Golden file snapshot tests
  - `run` — **Main development script** (run `./run` with no args to see all commands)
- `wasp-app-runner/` — Node.js CLI for running Wasp apps in e2e tests
- `web/` — Documentation website (Docusaurus), deployed to wasp.sh
- `mage/` — Archived GPT app generator for Wasp DSL apps from a description. Do not update it unless the task explicitly targets Mage.
- `examples/` — Tutorial and example apps (kitchen-sink, waspello, etc.)
- `scripts/` — Mon
```

</details>
