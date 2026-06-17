---
name: 0xtoools__0xtools
source: https://github.com/0xtoools/0xtools/blob/2639eb2bea5925d2a8daff0a8fb701e6667690f8/Claude.md
repo: 0xtoools/0xtools
kind: claude-md
stars: 2
last_pushed: 2026-06-10T13:05:50Z
license: mit
score: 9
domains: [cli-tools, blockchain, security]
tags: [solidity, rust, vscode-extension]
curated: 2026-06-15
curated_by: config-scout
---

# 0xtoools/0xtools — claude-md

**Why it's worth keeping:** It includes a 'Patterns to Follow' section that enforces specific logic (caching/debouncing) and strict dependency constraints to prevent bloat.

**Summary:** A dense architectural overview detailing a multi-tier compilation system and specialized Rust backend.

**Source credibility:** High-quality, highly technical documentation for a specialized blockchain security tool.

**Recency:** Very current, utilizing modern workflows like pnpm and Rust-based execution.

**Source:** [0xtoools/0xtools/Claude.md](https://github.com/0xtoools/0xtools/blob/2639eb2bea5925d2a8daff0a8fb701e6667690f8/Claude.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# 0xTools

Solidity smart contract analysis tool — VS Code extension + CLI. Extracts function selectors, event topics, error selectors, and provides real-time gas estimation with inline decorations.

## Quick Start

```bash
pnpm install                    # Install deps
pnpm run compile                # Build (webpack, production)
cd runner && cargo build        # Build Rust runner (optional)
pnpm test                       # Run tests (jest)
npx tsc --noEmit                # Type-check only
```

## Architecture

```
User → Extension (VS Code) / CLI
         ↓
     Core Engine: scanner → parser → cache → exporter
         ↓
     Features: realtime → compilation-service → [Runner | Forge | Solc]
         ↓
     Analysis: gas, storage-layout, call-graph, deployment, complexity, size
```

**Three-tier compilation backend** (priority order):
1. **Runner** — Rust binary (`runner/src/`), deploys contracts in revm, executes functions for real gas
2. **Forge** — Shells out to `forge build` for Foundry projects
3. **Solc-JS** — WASM compiler, universal fallback

If all compilation fails, regex fallback still extracts selectors (gas shows N/A).

## Directory Map

| Path | What |
|------|----
```

</details>
