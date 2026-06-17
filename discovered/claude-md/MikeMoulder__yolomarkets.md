---
name: MikeMoulder__yolomarkets
source: https://github.com/MikeMoulder/yolomarkets/blob/f937acd5bfca73451386d52913f81712a68bb9b8/CLAUDE.md
repo: MikeMoulder/yolomarkets
kind: claude-md
stars: 0
last_pushed: 2026-06-14T16:19:52Z
license: unknown
score: 10
domains: [blockchain, smart-contracts, ai-agents]
tags: [web3, foundry, troubleshooting, context-injection]
curated: 2026-06-16
curated_by: config-scout
---

# MikeMoulder/yolomarkets — claude-md

**Why it's worth keeping:** Includes 'Arc-specific gotchas' that document why standard tools (Foundry/Python) fail in this ecosystem and provides immediate code-level workarounds.

**Summary:** Provides high-density technical reality checks for a specific blockchain environment to prevent LLM hallucinations regarding gas, decimals, and tool behavior.

**Source credibility:** High technical depth suggests an experienced developer, despite the low star count.

**Recency:** Extremely current; addresses modern toolchain behaviors like TLS fingerprinting and EVM precompile mismatches.

**Source:** [MikeMoulder/yolomarkets/CLAUDE.md](https://github.com/MikeMoulder/yolomarkets/blob/f937acd5bfca73451386d52913f81712a68bb9b8/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# YOLO Markets — Agent guidance

A prediction-market platform on Arc testnet with an autonomous trading agent.
Full vision in [idea.md](idea.md). This file is the load-bearing context for
any AI agent (Claude Code, Cursor, …) working in this repo.

## Hard facts (don't re-derive)

| Thing | Value |
| --- | --- |
| Chain | Arc Testnet, chain ID `5042002` (`0x4CEF52`) |
| RPC (public) | `https://rpc.testnet.arc.network` |
| RPC (canteen) | `arc-canteen rpc-url` (token-gated, used by tooling) |
| Explorer | https://testnet.arcscan.app |
| Faucet | https://faucet.circle.com |
| USDC ERC-20 | `0x3600000000000000000000000000000000000000` — **6 decimals** |
| USDC native gas | same underlying, **18 decimals**, used to pay gas |
| EURC | `0x89B50855Aa3bE2F677cD6303Cec089B5F319D72a` (6 decimals) — unused for MVP |
| USYC | `0xe9185F0c5F296Ed1797AaE4238D26CCaBEadb86C` — **gated**, see below |
| Permit2 | `0x000000000022D473030F116dDEE9F6B43aC78BA3` |
| Multicall3 | `0xcA11bde05977b3631167028862bE2a173976CA11` |

## Plan deltas from idea.md (read before quoting idea.md to the user)

1. **USDC is the native gas token on Arc.** Idea.md frames USDC only as the
   settlement asset; on Arc it is a
```

</details>
