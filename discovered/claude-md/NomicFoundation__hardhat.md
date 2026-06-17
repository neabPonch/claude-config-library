---
name: NomicFoundation__hardhat
source: https://github.com/NomicFoundation/hardhat/blob/45b8cf3c3e40e65e78db30aa5f54e67a99ded2d9/CLAUDE.md
repo: NomicFoundation/hardhat
kind: claude-md
stars: 8483
last_pushed: 2026-06-13T21:43:22Z
license: other
score: 9
domains: [cli-tools, blockchain, typescript]
tags: [architecture, strict-rules, module-system]
curated: 2026-06-15
curated_by: config-scout
---

# NomicFoundation/hardhat — claude-md

**Why it's worth keeping:** It defines high-signal 'negative constraints' (e.g., what not to throw/import) and provides the exact logic needed for complex async import decisions.

**Summary:** Provides strict architectural constraints regarding error handling and complex module import patterns to maintain codebase stability.

**Source credibility:** High; Hardhat is a standard-setting development tool in the Ethereum ecosystem with significant community backing.

**Recency:** Very current, referencing 'Hardhat 3' and modern pnpm workflows.

**Source:** [NomicFoundation/hardhat/CLAUDE.md](https://github.com/NomicFoundation/hardhat/blob/45b8cf3c3e40e65e78db30aa5f54e67a99ded2d9/CLAUDE.md) · 8483★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Commands

Install - pnpm install

Build - pnpm build

Test - pnpm test

For single-file work, run these from the repo root. They build upstream deps and run the tool on the given path(s):

Lint single file - `pnpm lint:file path/to/file.ts` (runs prettier --check + eslint; pass `--fix` to auto-apply fixes)

Test single file - `pnpm test:file path/to/test.ts`

Test single test - add `.only` to the test, then `pnpm test:file --only path/to/test.ts`

Spellcheck single file - `pnpm spellcheck:file path/to/file.md`

## Repository layout

packages/\* – publishable packages

packages/hardhat - core logic and cli

## Rules

**Package structure** — Exported code and types (via `package#exports`) live under `src/`, non-exported internals under `src/internal/`.

**`hardhat-utils` first** — Before using `node:fs` or writing a utility, check `@nomicfoundation/hardhat-utils`. It covers fs, crypto, hex, error handling, and more.

**Errors** — Only throw `HardhatError`. Never `throw new Error()`. Use `HardhatError.isHardhatError()` (not `instanceof`) and `ensureError()` in catch clauses. `./scripts` is exempt.

### Using imports correctly in Hardhat 3

Use `await import` only if one of these co
```

</details>
