---
name: rainbow-me__browser-extension
source: https://github.com/rainbow-me/browser-extension/blob/5caa9e2aaef2e28367d2e5c06f0b95db98e40451/CLAUDE.md
repo: rainbow-me/browser-extension
kind: claude-md
stars: 193
last_pushed: 2026-06-08T18:12:53Z
license: gpl-3.0
score: 9
domains: [web-frontend, blockchain, security]
tags: [manifest-v3, react, typescript, chrome-extension, testing]
curated: 2026-06-15
curated_by: config-scout
---

# rainbow-me/browser-extension — claude-md

**Why it's worth keeping:** Provides specific feature-addition workflows, critical environment variable requirements (SECURE_WALLET_HASH_KEY), and known friction points like the Chrome version requirement.

**Summary:** A comprehensive guide that bridges high-level architecture with low-level environment 'gotchas' essential for an AI agent.

**Source credibility:** High; Rainbow is a major production Ethereum wallet with active development and high GitHub visibility.

**Recency:** Current; includes modern setup instructions for Yarn Berry/Corepack and specific Node/Chrome versions.

**Source:** [rainbow-me/browser-extension/CLAUDE.md](https://github.com/rainbow-me/browser-extension/blob/5caa9e2aaef2e28367d2e5c06f0b95db98e40451/CLAUDE.md) · 193★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Repository Overview

Rainbow is a cryptocurrency wallet browser extension built with TypeScript, React, and Manifest V3. It supports multiple blockchain networks, hardware wallets, and provides a comprehensive DeFi experience.

## Common Development Commands

### Setup & Installation

```bash
# Install dependencies and set up the project
yarn install
yarn setup
```

### Development

```bash
# Start development build with hot reload
yarn dev

# Build production extension
yarn build
```

### Testing

```bash
# Run unit/integration tests
yarn test

# Run specific E2E test suites (requires yarn build first)
yarn e2e:parallel     # Parallel E2E tests
yarn e2e:serial       # Serial E2E tests
yarn e2e:swap         # Swap feature tests
yarn e2e:send         # Send feature tests
yarn e2e:send:optimism # Optimism send tests
yarn e2e:dappInteractions # DApp interaction tests
yarn e2e serial/send/1_sendFlow.test.ts
```

### Code Quality

```bash
# Run linter
yarn lint

# Run type checking
yarn typecheck

# Both should pass before committing changes
```

## Architecture Overview

### Entry Points (`/src/entries/`)

- **background/**: Service worker handling extension lifecycle,
```

</details>
