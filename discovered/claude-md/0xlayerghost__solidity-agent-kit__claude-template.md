---
name: 0xlayerghost__solidity-agent-kit__claude-template
source: https://github.com/0xlayerghost/solidity-agent-kit/blob/c003c2146229af5349e1bf05d0dee30bb80b3d2f/CLAUDE.md.template
repo: 0xlayerghost/solidity-agent-kit
kind: claude-md
stars: 4
last_pushed: 2026-06-13T07:06:28Z
license: mit
score: 9
domains: [blockchain, smart-contracts, security, solidity]
tags: [foundry, security-first, mcp-optimized, defi]
curated: 2026-06-15
curated_by: config-scout
---

# 0xlayerghost/solidity-agent-kit — claude-md

**Why it's worth keeping:** The pattern of requiring specific 'skill' calls before critical actions (deploying, testing, debugging) creates a reliable procedural guardrail, while the explicit '.env' security restriction is a professional-grade safety rule.

**Summary:** A highly specialized instruction set for Solidity development that enforces a security-first workflow via mandatory skill invocations and tool usage.

**Source credibility:** Highly credible; part of a specialized developer kit with recent maintenance.

**Recency:** Current; incorporates modern MCP tool workflows and Foundry tooling.

**Source:** [0xlayerghost/solidity-agent-kit/CLAUDE.md.template](https://github.com/0xlayerghost/solidity-agent-kit/blob/c003c2146229af5349e1bf05d0dee30bb80b3d2f/CLAUDE.md.template) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project Rules

## Skill Auto-Invoke Rules

Before writing or modifying any Solidity contract (.sol files), you MUST invoke:
- /solidity-coding
- /solidity-security
- When creating NEW contracts from scratch, prefer using OpenZeppelinContracts MCP tools (solidity-erc20, solidity-erc721, etc.) to generate the base contract, then customize with /solidity-coding rules

Before writing or modifying proxy/upgradeable contracts, you MUST invoke:
- /solidity-coding
- /solidity-security
- /solidity-deploy
- /defi-security

Before writing or modifying test files (*.t.sol), you MUST invoke:
- /solidity-testing

Before deploying contracts or writing deployment scripts (*.s.sol), you MUST invoke:
- /solidity-deploy
- /defi-security

Before any on-chain operation (cast send, forge script --broadcast), you MUST invoke:
- /solidity-checklist

Before debugging failed on-chain transactions, you MUST invoke:
- /solidity-debug

Before conducting security audits or code reviews, you MUST:
- Run slither MCP analysis on the project first (if available) to get automated findings
- Then invoke /solidity-audit for manual checklist review
- Cross-reference both results for comprehensive coverage

Before cr
```

</details>
