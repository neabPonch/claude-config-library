---
name: helius-labs__core-ai__claude
source: https://github.com/helius-labs/core-ai/blob/8ce8bf96c9b2ebe5149442920bb7e66015860845/helius-cli/CLAUDE.md
repo: helius-labs/core-ai
kind: claude-md
stars: 19
last_pushed: 2026-06-11T16:21:04Z
license: mit
score: 9
domains: [cli-tools, blockchain, infrastructure]
tags: [command-pattern, error-handling, typescript, solana]
curated: 2026-06-15
curated_by: config-scout
---

# helius-labs/core-ai — claude-md

**Why it's worth keeping:** It defines a strict 'Command Pattern' and provides an exact protocol for extending the system (e.g., adding new error codes), which prevents architectural drift.

**Summary:** Provides a rigorous operational manual for executing commands, managing API resolution, and standardizing error classification.

**Source credibility:** High; official tooling from Helius, a major Solana infrastructure provider.

**Recency:** Current; references specific v1.3 updates and modern TypeScript patterns.

**Source:** [helius-labs/core-ai/helius-cli/CLAUDE.md](https://github.com/helius-labs/core-ai/blob/8ce8bf96c9b2ebe5149442920bb7e66015860845/helius-cli/CLAUDE.md) · 19★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# helius-cli

CLI tool for managing Helius accounts and querying Solana blockchain data via the Helius platform.

## Directory Structure

```
bin/helius.ts          # Entry point — Commander.js program, registers all commands
src/
  commands/            # One file per command group
    balance.ts         # balance, tokens, token-holders
    tx.ts              # tx parse, tx history, tx fees
    asset.ts           # 12 DAS API subcommands
    account.ts         # account info
    network-status.ts  # network status
    block.ts           # block by slot
    wallet.ts          # Wallet API (REST, not SDK) — identity, balances, history, transfers, funded-by
    webhook.ts         # webhook CRUD
    program.ts         # program accounts
    stake.ts           # staking commands
    zk.ts              # 24 ZK compression subcommands
    send.ts            # tx helpers (broadcast, raw, sender, poll, compute-units)
    reclaim.ts         # close empty SPL token accounts, reclaim rent (via Sender)
    ws.ts              # WebSocket streaming (account, logs, slot, signature, program)
    config-cmd.ts      # config show/set-api-key/set-network/set-project/clear
    signup.ts          # acco
```

</details>
