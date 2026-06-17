---
name: hypermesh-online__hypermesh
source: https://github.com/hypermesh-online/hypermesh/blob/ad06ee8a80a46e7a0f05a53e3a4469d768ad44de/CLAUDE.md
repo: hypermesh-online/hypermesh
kind: claude-md
stars: 7
last_pushed: 2026-06-05T01:30:31Z
license: other
score: 9
domains: [distributed-systems, blockchain, security]
tags: [protocol-driven, status-tracking, technical-debt]
curated: 2026-06-15
curated_by: config-scout
---

# hypermesh-online/hypermesh — claude-md

**Why it's worth keeping:** The 'Hard Protocol Requirements' section includes a meta-instruction for how to evolve the document itself when new rules emerge; the architecture table maps implementation percentages directly against critical technical gaps.

**Summary:** A high-rigor specification that combines strict protocol requirements with real-time development progress tracking across a complex monorepo.

**Source credibility:** High-density engineering documentation from an active distributed systems/Web3 project.

**Recency:** Highly current, referencing modern primitives like eBPF, Kyber-1024, and BLAKE3.

**Source:** [hypermesh-online/hypermesh/CLAUDE.md](https://github.com/hypermesh-online/hypermesh/blob/ad06ee8a80a46e7a0f05a53e3a4469d768ad44de/CLAUDE.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Web3 Ecosystem - Development Project Context

## Hard Protocol Requirements

**Canonical source**: `papers/HYPERMESH.md` Section 3 (Protocol Requirements), R1-R14.

**RULE**: Whenever the user says "this is a hard requirement" (or equivalent), check if it's already in `papers/HYPERMESH.md` Section 3. If not, add it as the next R-number. Keep requirements concrete and testable. Update this section's summary when requirements change.

**Current requirements (R1-R16)**:
- **R1** Sovereign genesis with asset instantiation — hardware assessed (not self-reported) as IPv6-addressed assets with Proof of State
- **R2** Four-proof authentication — PoSpace/PoStake/PoWork/PoTime on every state claim, binary authentic/not
- **R3** Pipeline ordering — Compress→Encrypt→Shard→Distribute, whole-blob encryption before sharding
- **R4** Content-addressed dedup — privacy-scoped reference tracking (full in Device/Private, none in Anonymous), tamper detection via BLAKE3 hash
- **R5** Erasure-coded redundancy — k-of-n reconstruction (default 10-of-14 Reed-Solomon)
- **R6** Instruction-based retrieval — shard maps under 1KB, receiver reconstructs
- **R7** Post-quantum storage encryption — Kyber-1024 KEM
```

</details>
