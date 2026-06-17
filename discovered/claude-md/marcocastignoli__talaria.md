---
name: marcocastignoli__talaria
source: https://github.com/marcocastignoli/talaria/blob/36cf0ed978aee4b6d3bc5bbbc5a418a199f35886/CLAUDE.md
repo: marcocastignoli/talaria
kind: claude-md
stars: 0
last_pushed: 2026-05-28T15:24:20Z
license: unknown
score: 9
domains: [web-frontend, blockchain-evm, dapp]
tags: [react-19, tailwind-v4, viem, evm]
curated: 2026-06-15
curated_by: config-scout
---

# marcocastignoli/talaria — claude-md

**Why it's worth keeping:** Includes critical 'gotchas' (like viem chainless requirements) that prevent AI-generated bugs, and uses a detailed folder map to facilitate efficient file discovery.

**Summary:** Provides deep architectural context and specific business logic for an EVM block explorer, including address labeling hierarchies. It functions as a high-density project bible that mitigates common library pitfalls.

**Source credibility:** High; the author is an expert in the niche domain of ERC-7730/Sourcify and the repo is actively maintained.

**Recency:** Very current; references React 19 and Tailwind v4.

**Source:** [marcocastignoli/talaria/CLAUDE.md](https://github.com/marcocastignoli/talaria/blob/36cf0ed978aee4b6d3bc5bbbc5a418a199f35886/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Instructions for Claude Code when working in this repo.

## What this is

**Talaria** — a clean, friendly EVM block-explorer + contract interaction tool.

Two ideas distinguish it from existing block explorers:

1. **ERC-7730 clear-signing everywhere.** Transactions render as sentences ("Send
   100 USDT to alice.eth") instead of decoded-but-unlabeled calldata. The Sourcify
   clear-signing registry provides per-contract descriptors; we just render them.
2. **Trustless client-side re-verification.** Sourcify says a contract is verified,
   but you don't have to trust that. The browser downloads the right Solidity
   compiler via [`web-solc`](https://www.npmjs.com/package/web-solc), recompiles
   the source in a Web Worker, and bytecode-matches against the chain.

The whole app is a PWA — no backend. The user brings their own RPC.

Production: https://talaria.castignoli.it/ (deployed via GH Pages on push to `main`).

## Stack

| Layer | Choice | Notes |
|---|---|---|
| Build | Vite + React 19 + TypeScript | |
| Styling | Tailwind v4 (`@tailwindcss/vite` plugin) | No PostCSS config; v4 reads `index.css` |
| UI primitives | Radix UI wrapped in shadcn-style components | Li
```

</details>
