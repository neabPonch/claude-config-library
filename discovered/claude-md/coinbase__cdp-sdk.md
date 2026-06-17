---
name: coinbase__cdp-sdk
source: https://github.com/coinbase/cdp-sdk/blob/76a73d8ec7b0f6080a11c0e6f6733e2c71a0ff86/CLAUDE.md
repo: coinbase/cdp-sdk
kind: claude-md
stars: 184
last_pushed: 2026-06-10T04:56:27Z
license: mit
score: 8
domains: [multi-language, sdk]
tags: [polyglot, monorepo, command-reference]
curated: 2026-06-15
curated_by: config-scout
---

# coinbase/cdp-sdk — claude-md

**Why it's worth keeping:** It effectively solves the polyglot problem by mapping specific build/test commands to their respective subdirectories, preventing tool mismatches during task execution.

**Summary:** Provides language-specific command suites and architectural overviews for a multi-language SDK repository.

**Source credibility:** High; maintained by Coinbase with active recent updates.

**Recency:** Current; utilizes modern tooling like uv and pnpm.

**Source:** [coinbase/cdp-sdk/CLAUDE.md](https://github.com/coinbase/cdp-sdk/blob/76a73d8ec7b0f6080a11c0e6f6733e2c71a0ff86/CLAUDE.md) · 184★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is the Coinbase Developer Platform (CDP) SDK repository containing multi-language client libraries for creating, managing, and using crypto wallets. The SDK supports TypeScript, Python, and Go implementations.

## Repository Structure

- `typescript/` - TypeScript/Node.js SDK implementation
- `python/` - Python SDK implementation
- `go/` - Go SDK implementation
- `rust/` - Rust SDK implementation
- `examples/` - Working examples for all languages
- `openapi.yaml` - OpenAPI specification for the CDP API

## Development Commands

### TypeScript (`typescript/` directory)

```bash
# Install dependencies
pnpm install

# Build the SDK
pnpm build

# Run tests
pnpm test

# Run E2E tests
pnpm test:e2e

# Lint code
pnpm lint

# Fix linting issues
pnpm lint:fix

# Format code
pnpm format

# Check formatting
pnpm format:check

# Generate docs
pnpm run docs

# Generate Markdown docs
pnpm run docs:md

# Generate OpenAPI client
pnpm orval
```

### Python (`python/` directory)

```bash
# Install dependencies (with dev dependencies)
uv sync

# Run tests
make test

#
```

</details>
