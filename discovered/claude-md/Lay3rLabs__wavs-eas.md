---
name: Lay3rLabs__wavs-eas
source: https://github.com/Lay3rLabs/wavs-eas/blob/0864497c1225cf4e2dc5092336c1b7fd91e4c7a8/claude.md
repo: Lay3rLabs/wavs-eas
kind: claude-md
stars: 0
last_pushed: 2025-08-08T13:53:31Z
license: mit
score: 8
domains: [blockchain, webassembly, smart-contracts]
tags: [rust, solidity, wasi, foundry]
curated: 2026-06-16
curated_by: config-scout
---

# Lay3rLabs/wavs-eas — claude-md

**Why it's worth keeping:** The 'Component Development' section provides essential trait/logic requirements for new components, which prevents the LLM from hallucinating incorrect implementations. It also clearly differentiates between building Solidity vs WASI components via specific make commands.

**Summary:** A comprehensive guide for a complex Web3 monorepo that covers architecture, multi-language build processes, and component implementation patterns.

**Source credibility:** Zero stars on GitHub, but the technical depth indicates a specialized engineering project.

**Recency:** 10 months old; remains highly relevant as it focuses on architectural patterns and tool orchestration rather than transient API versions.

**Source:** [Lay3rLabs/wavs-eas/claude.md](https://github.com/Lay3rLabs/wavs-eas/blob/0864497c1225cf4e2dc5092336c1b7fd91e4c7a8/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

The spec is `SPEC.md`.

## Project Overview

This is a WAVS (WebAssembly AVS) monorepo template that integrates with Ethereum Attestation Service (EAS) for building verifiable offchain applications. The project combines:

- **Solidity contracts** for blockchain interaction (EAS attestations, triggers, submissions)
- **Rust WASI components** for WebAssembly execution in the WAVS runtime
- **TypeScript/JavaScript components** for alternative WASI implementations
- **Foundry** for Solidity development and testing
- **Docker** for containerized services and deployment

## Architecture

The system follows a trigger-response pattern:
1. **Trigger contracts** emit events that WAVS monitors
2. **WASI components** process these events and perform computations
3. **Submission contracts** receive and store results from WAVS operators
4. **EAS integration** enables attestation-based workflows

Key directories:
- `src/` - Solidity contracts (triggers, submissions, EAS integration)
- `docs/` - Documentation for WAVS
- `components/` - WASI components in Rust and TypeScript
- `test/
```

</details>
