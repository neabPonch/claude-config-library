---
name: dangmai__prettier-plugin-apex
source: https://github.com/dangmai/prettier-plugin-apex/blob/8ccdd2c270d6fa1cecc8ebdd1cae9ff159691e18/CLAUDE.md
repo: dangmai/prettier-plugin-apex
kind: claude-md
stars: 269
last_pushed: 2026-06-15T04:45:51Z
license: mit
score: 9
domains: [cli-tools, compiler-tooling, monorepo]
tags: [tdd, nx, prettier, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# dangmai/prettier-plugin-apex — claude-md

**Why it's worth keeping:** It enforces strict TDD patterns (fixture requirements), defines exact triggers for changelog updates, and includes high-signal validation commands like AST comparison to prevent regressions.

**Summary:** Provides rigorous operational instructions for a TypeScript/Java monorepo involving specific testing modes and verification steps.

**Source credibility:** High; comes from a specialized, actively maintained open-source tool with specific technical constraints.

**Recency:** Very current; the repository is actively maintained (0 months ago).

**Source:** [dangmai/prettier-plugin-apex/CLAUDE.md](https://github.com/dangmai/prettier-plugin-apex/blob/8ccdd2c270d6fa1cecc8ebdd1cae9ff159691e18/CLAUDE.md) · 269★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# prettier-plugin-apex

A Prettier plugin for Salesforce Apex. It is a pnpm monorepo orchestrated with Nx. The plugin delegates parsing to a Java component (`apex-ast-serializer`) that wraps Salesforce's proprietary `jorje` parser, then uses Prettier's doc IR to format the resulting AST.

## Read these first

- [CONTRIBUTING.md](CONTRIBUTING.md) — full dev setup, quickstart, and workflow
- [packages/prettier-plugin-apex/README.md](packages/prettier-plugin-apex/README.md) — plugin usage and options
- [packages/apex-ast-serializer/README.md](packages/apex-ast-serializer/README.md) — Java parser, jorje dependency, type generation

## Monorepo structure

```
packages/
  prettier-plugin-apex/      # TypeScript plugin (parser.ts, printer.ts, comments.ts)
  apex-ast-serializer/       # Java/Gradle parser wrapping jorje
  playground/                # React/Vite web playground (deployed on Render)
  @prettier-apex/            # Platform-specific native binary packages
```

## Key commands

```bash
# Start HTTP parsing server (needed for built-in mode; VSCode task does this automatically)
pnpm nx run prettier-plugin-apex:start-server

# Run unit tests (built-in HTTP server mode — preferred f
```

</details>
