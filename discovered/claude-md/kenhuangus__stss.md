---
name: kenhuangus__stss
source: https://github.com/kenhuangus/stss/blob/0cff0de34eae665ad6afa7d79d8938652bea53eb/claude.md
repo: kenhuangus/stss
kind: claude-md
stars: 7
last_pushed: 2026-03-19T14:59:22Z
license: unknown
score: 9
domains: [security, cli-tools, typescript]
tags: [technical-specification, algorithm-driven]
curated: 2026-06-15
curated_by: config-scout
---

# kenhuangus/stss — claude-md

**Why it's worth keeping:** It treats the instruction file as a formal spec, providing complete TypeScript interfaces and step-by-step algorithmic logic (e.g., specific Merkle tree node construction) to eliminate LLM ambiguity.

**Summary:** A high-density technical specification that defines exact data structures, cryptographic algorithms, and security scanning rules.

**Source credibility:** A specialized security tool with technical depth demonstrated through complex implementation details.

**Recency:** Current; utilizes modern tech stacks like pnpm workspaces, Vitest, and @noble/ed25519.

**Source:** [kenhuangus/stss/claude.md](https://github.com/kenhuangus/stss/blob/0cff0de34eae665ad6afa7d79d8938652bea53eb/claude.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# STSS — Skill Trust & Signing Service
## Implementation Guide for Claude Code

---

## Mission

Build the **Skill Trust & Signing Service (STSS)**: a security layer for AI agent skill ecosystems (Claude Code, OpenClaw, IDE agents). STSS scans skill folders for threats, computes cryptographic integrity proofs, and issues signed attestations that can be verified before skills are loaded.

**Core constraint**: Never modify host application code. STSS works entirely by controlling what enters skill directories.

---

## Repo Structure

```
stss/
├── packages/
│   ├── core/          # Scanner, Policy, Hasher, Merkle, Signer, Verifier, LLM Auditor
│   ├── cli/           # stss CLI binary
│   ├── hub/           # stss-hub wrapper CLI (install, update, batch scan)
│   └── hooks/         # Git hook installer + CI workflow templates
├── package.json       # pnpm workspace root
├── pnpm-workspace.yaml
├── tsconfig.base.json
└── README.md
```

---

## Technology Stack

- **Language**: TypeScript, strict mode throughout
- **Package manager**: pnpm with workspaces
- **Validation**: Zod for all external data (policy YAML, attestation JSON, findings)
- **Testing**: Vitest
- **CLI framework**: com
```

</details>
