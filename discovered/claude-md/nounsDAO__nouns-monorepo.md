---
name: nounsDAO__nouns-monorepo
source: https://github.com/nounsDAO/nouns-monorepo/blob/86a781ecf199cd26825c047c94b9b4946b73ff04/CLAUDE.md
repo: nounsDAO/nouns-monorepo
kind: claude-md
stars: 685
last_pushed: 2026-06-08T21:25:47Z
license: gpl-3.0
score: 9
domains: [web-frontend, blockchain, monorepo]
tags: [monorepo, web3, migration-guide, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# nounsDAO/nouns-monorepo — claude-md

**Why it's worth keeping:** The explicit migration guides (Redux to TanStack/CSS Modules to Tailwind) prevent the AI from suggesting outdated patterns. Package-specific command blocks and environment variable lists ensure high accuracy in task execution within a monorepo.

**Summary:** Provides deep context for a complex monorepo by detailing build dependencies, package-specific commands, and crucial architecture migrations.

**Source credibility:** Highly credible; Nouns DAO is a major, well-maintained open-source project with significant community backing.

**Recency:** Extremely current; reflects modern toolchains and ongoing active migrations.

**Source:** [nounsDAO/nouns-monorepo/CLAUDE.md](https://github.com/nounsDAO/nouns-monorepo/blob/86a781ecf199cd26825c047c94b9b4946b73ff04/CLAUDE.md) · 685★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Architecture

This is a monorepo for Nouns DAO, a generative avatar art collective run by crypto misfits. The project uses:
- **pnpm** as the package manager (required version 10.10.0+)
- **Turbo** for monorepo build orchestration
- **TypeScript** throughout the codebase
- **Node.js** 16.x or higher

## Package Structure

Five main packages with interdependencies:

1. **nouns-assets** - PNG and run-length encoded Noun image data
2. **nouns-contracts** - Solidity smart contracts for Nouns DAO (uses Hardhat + Foundry)
3. **nouns-sdk** - Contract addresses, ABIs, instances, and image utilities
4. **nouns-webapp** - React frontend (Vite + Tailwind + i18n)
5. **nouns-subgraph** - The Graph subgraph manifests

Build dependencies: webapp depends on assets → contracts → sdk.

## Essential Commands

### Development
```bash
pnpm install          # Install all dependencies
pnpm dev              # Start development servers (builds dependencies first)
pnpm build            # Build all packages
pnpm test             # Run tests across all packages
```

### Code Quality
```

</details>
