---
name: nicolaslara__solana-noir-verifier
source: https://github.com/nicolaslara/solana-noir-verifier/blob/42d00736399efc6d5784523bd8a71cc7e36c58de/claude.md
repo: nicolaslara/solana-noir-verifier
kind: claude-md
stars: 4
last_pushed: 2026-03-29T09:26:49Z
license: unknown
score: 9
domains: [blockchain, cryptography, rust, solana]
tags: [zk-proofs, solana-program, noir, rust, security-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# nicolaslara/solana-noir-verifier — claude-md

**Why it's worth keeping:** It uses 'Critical Development Rules' to preemptively address common high-stakes errors like incorrect serialization or compute limit failures. The inclusion of specific instruction codes and a detailed memory/account map is excellent for LLM accuracy in complex systems.

**Summary:** A highly specialized technical guide for zero-knowledge proof verification on Solana using Noir/UltraHonk. It maps out complex architectural requirements including account structures, serialization formats, and phased transaction workflows.

**Source credibility:** High-quality niche repository focused on advanced blockchain cryptography.

**Recency:** Current; aligned with recent Solana development standards and toolchains.

**Source:** [nicolaslara/solana-noir-verifier/claude.md](https://github.com/nicolaslara/solana-noir-verifier/blob/42d00736399efc6d5784523bd8a71cc7e36c58de/claude.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Development Guide for Solana Noir Verifier

This file contains essential context and rules for working on the Solana Noir Verifier project.

## ⚠️ IMPORTANT: Always Check Cursor Rules

**Before starting any work**, you MUST:

1. **Read the active Cursor rules** in `.cursor/rules/`:
   - `ultrahonk-development.mdc` - Development patterns for Rust/Solana BN254
   - `ultrahonk-workflow.mdc` - Main development workflow
   - `ultrahonk-references.mdc` - External references and resources

2. **Follow the patterns** defined in those rules for:
   - VK registry pattern (load from account, not embedded)
   - Account structure and sizes
   - BN254 syscall usage
   - Field/curve serialization formats
   - Phased verification workflow
   - Instruction codes

3. **Note**: Files ending in `.mdc.disabled` are inactive (UltraPlonk rules are disabled)

The sections below consolidate key information from those rules for quick reference, but you should always verify against the source `.cursor/rules/` files when making changes.

## Project Overview

A circuit-specific verifier for Noir zero-knowledge proofs on Solana, using UltraHonk proving system with Solana's native BN254 syscalls.

**Sta
```

</details>
