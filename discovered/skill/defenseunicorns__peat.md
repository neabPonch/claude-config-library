---
name: defenseunicorns__peat
source: https://github.com/defenseunicorns/peat/blob/965e2bb0bed458220e73ba3f4477cb46cf02fc45/SKILL.md
repo: defenseunicorns/peat
kind: skill
stars: 19
last_pushed: 2026-06-15T02:59:53Z
license: apache-2.0
score: 9
domains: [rust, security, embedded-systems, architecture]
tags: [orchestrator, multi-repo, invariants, rust]
curated: 2026-06-16
curated_by: config-scout
---

# defenseunicorns/peat — skill

**Why it's worth keeping:** The 'Skill Router' table is a perfect template for navigating large/multi-repo projects, and the 'Hard Invariants' section provides high-density constraints that prevent subtle architectural drift.

**Summary:** A high-level orchestrator skill that uses a 'Skill Router' pattern to manage agent navigation across a complex multi-repo ecosystem. It enforces strict architectural and security invariants (like FIPS crypto requirements) globally.

**Source credibility:** High; Defense Unicorns is a reputable organization specialized in mission-critical defense software.

**Recency:** Very current; reflects modern Rust patterns, FFI/UniFFI workflows, and contemporary security standards.

**Source:** [defenseunicorns/peat/SKILL.md](https://github.com/defenseunicorns/peat/blob/965e2bb0bed458220e73ba3f4477cb46cf02fc45/SKILL.md) · 19★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: peat-ecosystem
description: Top-level skill for Claude Code sessions across any peat-* repo. Read first, then read the per-repo SKILL.md.
when_to_use: Any session touching files in a defenseunicorns/peat-* repository, or coordinating changes across more than one peat repo.
verifies_with: Each affected repo's CI green, no architecture invariant violated, PR references its issue with the required sections.
---

# Peat Ecosystem SKILL

Peat is an interoperability-first mesh registry sync platform built for heterogeneous autonomous systems in defense and edge environments. Its core value proposition is **interoperability that enables scale** — Peat connects systems that don't speak the same language across transport and protocol boundaries. Peat is developed under the Defense Unicorns GitHub org: https://github.com/defenseunicorns

## When this skill applies

- Any session touching files in a `peat-*` repo or the top-level `peat` crate
- Cross-repo changes affecting more than one peat repo
- Reviewing a PR in any peat repo

After reading this file, read the relevant per-repo SKILL.md from the router below. Per-repo skills are authored against `peat/SKILL_TEMPLATE.md`.

## Ski
```

</details>
