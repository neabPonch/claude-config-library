---
name: renlabs-dev__torus-ts__claude
source: https://github.com/renlabs-dev/torus-ts/blob/3ae3e4d95e5c3c65d7978c0c7d791ba75a91b587/packages/torus-sdk-ts/src/chain/CLAUDE.md
repo: renlabs-dev/torus-ts
kind: claude-md
stars: 16
last_pushed: 2026-06-09T14:04:36Z
license: unknown
score: 8
domains: [blockchain, typescript, backend-api]
tags: [zod, type-safety, error-handling, substrate]
curated: 2026-06-15
curated_by: config-scout
---

# renlabs-dev/torus-ts — claude-md

**Why it's worth keeping:** Provides a clear 'Schema -> Infer Type -> Query Function' workflow that ensures type safety across external data boundaries. Includes detailed instructions on transitioning to Result types for better error management.

**Summary:** Defines rigorous architectural standards for creating blockchain modules using Zod schemas and consistent error-handling patterns.

**Source credibility:** Technical depth suggests highly specialized domain knowledge in Substrate/Blockchain development despite lower star count.

**Recency:** Extremely current; uses modern TypeScript and Zod practices.

**Source:** [renlabs-dev/torus-ts/packages/torus-sdk-ts/src/chain/CLAUDE.md](https://github.com/renlabs-dev/torus-ts/blob/3ae3e4d95e5c3c65d7978c0c7d791ba75a91b587/packages/torus-sdk-ts/src/chain/CLAUDE.md) · 16★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Torus SDK core Substrate modules

Core modules for interacting with the Torus Substrate blockchain pallets. Each
module provides Zod schemas, TypeScript type definitions, query and transaction
functions, and utilities for a specific pallet.

## Module Overview

All modules follow consistent patterns:

- **Zod Schema Validation**
  - Substrate type parsers defined using `sb_` prefixed utilities
- **Type Inference**
  - Types inferred from Zod schemas using `z.infer<typeof SCHEMA>`
- **Error Handling**
  - Robust error handling with `tryAsync` and `trySync` wrappers etc
- **Query Functions**
  - Standardized functions for blockchain data retrieval

## Files

- [@common/] - Shared utilities and types for storage map parsing
  - `index.ts` - Re-exports and common types
  - `storage-maps.ts` - Storage map handling utilities
- [@balance.ts] - System and balances pallet queries
- [@emission0.ts] - Emission0 pallet interface (emission parameters, weights)
- [@governance.ts] - Governance pallet interface (proposals, voting,
  applications)
- [@permission0.ts] - Permission0 pallet interface (delegation permissions)
- [@torus0/] - Torus0 pallet interface (organized by domain)
  - `agents.ts
```

</details>
