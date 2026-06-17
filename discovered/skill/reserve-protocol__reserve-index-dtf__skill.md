---
name: reserve-protocol__reserve-index-dtf__skill
source: https://github.com/reserve-protocol/reserve-index-dtf/blob/ba1088fbb618abdbb9d2cfcefc3ebcd5b70cbac1/.claude/skills/release-changes/SKILL.md
repo: reserve-protocol/reserve-index-dtf
kind: skill
stars: 37
last_pushed: 2026-06-15T17:45:33Z
license: mit
score: 8
domains: [blockchain, smart-contracts, devops, qa]
tags: [git-diff, solidity, changelog]
curated: 2026-06-16
curated_by: config-scout
---

# reserve-protocol/reserve-index-dtf — skill

**Why it's worth keeping:** Demonstrates high-level noise reduction by explicitly instructing the agent to ignore internal implementation details and focus only on interface/caller impact.

**Summary:** Automates the extraction of breaking changes in Solidity contracts between Git tags for frontend developers.

**Source credibility:** High; comes from a legitimate DeFi protocol (Reserve) with active development.

**Recency:** Current; relies on standard Git and shell utilities compatible with modern CLI environments.

**Source:** [reserve-protocol/reserve-index-dtf/.claude/skills/release-changes/SKILL.md](https://github.com/reserve-protocol/reserve-index-dtf/blob/ba1088fbb618abdbb9d2cfcefc3ebcd5b70cbac1/.claude/skills/release-changes/SKILL.md) · 37★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: release-changes
description: Analyze contract changes between two release tags (struct changes, deployer changes, recommendations)
argument-hint: "<from-tag> <to-tag> (e.g. r4.0.0 r5.0.0)"
disable-model-invocation: true
allowed-tools: Bash(git diff *), Bash(git log *), Bash(git tag *), Bash(git rev-parse *), Bash(git show *), Read, Grep, Glob
---

# Frontend Changes Analysis

Analyze Solidity contract changes between two release tags. Produce a concise report of what a frontend developer needs to know.

## Configuration

- **Arguments**: `$ARGUMENTS` — two space-separated tags: `<from-tag> <to-tag>` (e.g. `r4.0.0 r5.0.0`)
- **from-tag**: The older release tag (baseline)
- **to-tag**: The newer release tag (target)
- **Diff scope**: `contracts/` directory only
- **Exclude**: `contracts/spells/`, `contracts/mocks/`, any `test/` paths

## Exported Contracts (Frontend-Facing)

| Contract           | Source File                                 |
| ------------------ | ------------------------------------------- |
| Folio              | `contracts/Folio.sol`                       |
| FolioLens          | `contracts/periphery/FolioLens.sol`         |
| GovernanceDeployer | `cont
```

</details>
