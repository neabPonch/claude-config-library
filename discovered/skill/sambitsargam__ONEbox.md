---
name: sambitsargam__ONEbox
source: https://github.com/sambitsargam/ONEbox/blob/61502ae9c6b0a6f47eedd1c69a6749f501c13db3/skill.md
repo: sambitsargam/ONEbox
kind: skill
stars: 0
last_pushed: 2026-03-27T09:28:58Z
license: mit
score: 8
domains: [blockchain, web3, fullstack-development, cli-tools]
tags: [onechain, move, dapp, deployment]
curated: 2026-06-17
curated_by: config-scout
---

# sambitsargam/ONEbox — skill

**Why it's worth keeping:** It uses a strong 'Agent Behavior Contract' to minimize turn-taking and provides explicit instructions for capturing deployment IDs to automate frontend wiring—a critical step in blockchain workflows.

**Summary:** A highly specialized skill file for end-to-end dApp development on the OneChain blockchain.

**Source credibility:** Low star count suggests it is likely a niche or early-stage ecosystem-specific tool.

**Recency:** Current; utilizes modern tech stacks like Vite, React-TS, and Move 2024 edition.

**Source:** [sambitsargam/ONEbox/skill.md](https://github.com/sambitsargam/ONEbox/blob/61502ae9c6b0a6f47eedd1c69a6749f501c13db3/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ONEbox
description: "Build production-style OneChain apps end-to-end with minimal back-and-forth: scaffold contracts + frontend, implement requested features, build, deploy, wire IDs, and run. Use when users say build/create/make an app, dApp, contract, dashboard, launchpad, NFT, DeFi, game, or full-stack project on OneChain."
---

# OneChain Full-Stack Builder Skill

Use this skill when a user asks to build any app on OneChain.

## Agent Behavior Contract

Follow these rules by default:

1. Start building immediately.
2. Ask questions only when a blocker prevents implementation.
3. If requirements are incomplete, assume practical defaults and continue.
4. Produce working code first, polish second.
5. After each milestone, run validation commands and fix failures.
6. Return a concise summary with deployed IDs, changed files, and run commands.

## Default Assumptions

If the user does not specify alternatives, use:

- Network: OneChain testnet
- RPC: `https://rpc-testnet.onelabs.cc:443`
- Explorer: `https://onescan.cc/testnet`
- Contract language: Move (`edition = "2024.beta"`)
- Frontend: React + TypeScript + Vite
- Wallet + chain libs: `@onelabs/dapp-kit`, `@mysten/sui`,
```

</details>
