---
name: plurigrid__asi__skill-bak
source: https://github.com/plurigrid/asi/blob/3f9ac1f363457424c7caaf0cf809f8a8873ecd78/skills/move-fuzzing/SKILL.md.bak
repo: plurigrid/asi
kind: skill
stars: 26
last_pushed: 2026-06-10T12:51:42Z
license: mit
score: 8
domains: [security, blockchain, smart-contracts]
tags: [move, fuzzing, aptos, sui, audit]
curated: 2026-06-17
curated_by: config-scout
---

# plurigrid/asi — skill

**Why it's worth keeping:** It provides actionable CLI command sequences, configuration schemas, and property-testing code patterns that an agent can directly implement to execute security audits.

**Summary:** A highly specialized technical protocol for fuzzing Move smart contracts across Aptos and Sui ecosystems.

**Source credibility:** High; leverages recognized industry tools like MoveSmith (Aptos Labs) and ItyFuzz.

**Recency:** Extremely current; recently updated and covers modern Move ecosystems.

**Source:** [plurigrid/asi/skills/move-fuzzing/SKILL.md.bak](https://github.com/plurigrid/asi/blob/3f9ac1f363457424c7caaf0cf809f8a8873ecd78/skills/move-fuzzing/SKILL.md.bak) · 26★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Move Smart Contract Fuzzing Skill

Comprehensive fuzzing toolkit for Move smart contracts on Aptos, Sui, and Movement chains.

## Trit Assignment: MINUS (-1) — Sink/Verification

Fuzzing is a verification sink that consumes contracts and emits vulnerability reports.

## Tools Overview

| Tool | Target | Engine | Features |
|------|--------|--------|----------|
| **MoveSmith** | Aptos (compiler/VM) | libFuzzer, AFL++, honggfuzz | V1/V2 diff, optimization diff |
| **sui-fuzzer** | Sui Move | Coverage-guided | Stateful fuzzing, property testing |
| **ItyFuzz** | EVM + MoveVM | LibAFL hybrid | Symbolic + fuzzing, flashloan, decompile |
| **Belobog** | Move (research) | Custom | Framework for vulnerability detection |

## Quick Start

### ItyFuzz (Most Versatile)

```bash
# Install
curl -L https://ity.fuzz.land/ | bash
ityfuzzup

# Fuzz Move contract on Sui
ityfuzz sui -t <package_id>::<module>::<function>

# Fuzz with onchain forking
ityfuzz sui -t <target> --onchain-block-number <block>
```

### MoveSmith (Aptos Compiler Fuzzing)

```bash
# Clone and build
git clone https://github.com/aptos-labs/move-smith
cd move-smith
make build-docker
./run make

# Run V1 vs V2 compiler different
```

</details>
