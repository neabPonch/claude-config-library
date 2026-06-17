---
name: lfglabs-dev__verity__skill
source: https://github.com/lfglabs-dev/verity/blob/9dd19fda97f21868456a12c63c00522a82f9a05e/docs-site/public/skill.md
repo: lfglabs-dev/verity
kind: skill
stars: 119
last_pushed: 2026-06-15T06:11:04Z
license: mit
score: 9
domains: [smart-contracts, formal-verification, security, blockchain]
tags: [lean4, evm, formal-verification, smart-contracts]
curated: 2026-06-15
curated_by: config-scout
---

# lfglabs-dev/verity — skill

**Why it's worth keeping:** It uses high-value negative constraints (e.g., 'Do not use sorry/admit') essential for formal verification and provides clear documentation discovery paths specific to LLM context window management.

**Summary:** Provides a rigorous procedural framework for an agent to author, port, and verify smart contracts using Lean 4 within the Verity ecosystem.

**Source credibility:** High; the repo shows active maintenance and addresses a highly technical, niche domain with precision.

**Recency:** Very current; utilizes modern agentic patterns like structured /llms.txt/discovery.

**Source:** [lfglabs-dev/verity/docs-site/public/skill.md](https://github.com/lfglabs-dev/verity/blob/9dd19fda97f21868456a12c63c00522a82f9a05e/docs-site/public/skill.md) · 119★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Verity Agent Skill

Use this skill when working in the Verity repository or docs. Verity is a Lean 4 framework for writing smart contracts that compile to EVM bytecode with machine-checked correctness proofs.

## First Principles

- Treat Lean files in `Contracts/<Name>/` as the source of truth.
- Keep specs, EDSL implementation, generated artifacts, and proofs aligned.
- Do not use `sorry`, `admit`, new `axiom`s, or unchecked assumptions to make proofs pass.
- Prefer existing Verity primitives and proof patterns before adding abstractions.
- Read `/llms.txt` first for the compact working model, then fetch `/llms-full.txt` when broader context is needed.

## Add A Contract

1. Scaffold with `python3 scripts/generate_contract.py <Name> --fields ... --functions ...` when the contract shape fits the generator.
2. Implement storage, specs, and EDSL functions under `Contracts/<Name>/`.
3. Register compiler integration following the existing contract examples.
4. Prove each public operation with the `_meets_spec` convention.
5. Run `lake build`.
6. If compiler behavior changes, run the relevant Foundry and property tests.

Primary docs:

- `/first-contract.md`
- `/guides/add-contract.m
```

</details>
