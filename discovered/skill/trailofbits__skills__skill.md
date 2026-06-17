---
name: trailofbits__skills__skill
source: https://github.com/trailofbits/skills/blob/c070b9b5881183ea5f6e320ff06c46688becb13e/plugins/building-secure-contracts/skills/solana-vulnerability-scanner/SKILL.md
repo: trailofbits/skills
kind: skill
stars: 5705
last_pushed: 2026-06-11T19:48:24Z
license: cc-by-sa-4.0
score: 9
domains: [security, blockchain, smart-contracts]
tags: [solana, rust, audit, security]
curated: 2026-06-15
curated_by: config-scout
---

# trailofbits/skills — skill

**Why it's worth keeping:** Includes actionable ripgrep commands for discovery and a strictly structured reporting template with attack scenarios and mitigations.

**Summary:** A highly specialized security auditing skill for Solana and Anchor programs that focuses on six critical vulnerability patterns.

**Source credibility:** High; written by Trail of Bits, a premier security research firm.

**Recency:** Current; covers modern Solana/Anchor patterns including sysvar and instruction introspection security.

**Source:** [trailofbits/skills/plugins/building-secure-contracts/skills/solana-vulnerability-scanner/SKILL.md](https://github.com/trailofbits/skills/blob/c070b9b5881183ea5f6e320ff06c46688becb13e/plugins/building-secure-contracts/skills/solana-vulnerability-scanner/SKILL.md) · 5705★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: solana-vulnerability-scanner
description: Scans Solana programs for 6 critical vulnerabilities including arbitrary CPI, improper PDA validation, missing signer/ownership checks, and sysvar spoofing. Use when auditing Solana/Anchor programs.
---

# Solana Vulnerability Scanner

## 1. Purpose

Systematically scan Solana programs (native and Anchor framework) for platform-specific security vulnerabilities related to cross-program invocations, account validation, and program-derived addresses. This skill encodes 6 critical vulnerability patterns unique to Solana's account model.

## 2. When to Use This Skill

- Auditing Solana programs (native Rust or Anchor)
- Reviewing cross-program invocation (CPI) logic
- Validating program-derived address (PDA) implementations
- Pre-launch security assessment of Solana protocols
- Reviewing account validation patterns
- Assessing instruction introspection logic

## 3. Platform Detection

### File Extensions & Indicators
- **Rust files**: `.rs`

### Language/Framework Markers
```rust
// Native Solana program indicators
use solana_program::{
    account_info::AccountInfo,
    entrypoint,
    entrypoint::ProgramResult,
    pubkey::Pubkey,
```

</details>
