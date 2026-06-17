---
name: gridaco__grida__skill
source: https://github.com/gridaco/grida/blob/5fcea20837f696e6071b01d79e92ce72006d5891/.agents/skills/sdk-seam/SKILL.md
repo: gridaco/grida
kind: skill
stars: 2522
last_pushed: 2026-06-14T12:46:58Z
license: apache-2.0
score: 9
domains: [software-architecture, api-design, multi-agent-systems]
tags: [sdk-seams, contract-enforcement, architectural-integrity]
curated: 2026-06-15
curated_by: config-scout
---

# gridaco/grida — skill

**Why it's worth keeping:** Uses a 'Maintainer' subagent profile to defend producer invariants and an intermediary artifact (FEEDBACKS.md) to prevent consumer-side coupling.

**Summary:** A multi-agent workflow designed to maintain clean API boundaries by treating internal dependency changes as formal, external feature requests.

**Source credibility:** High; derived from Grida, a highly-starred open design project with active maintenance.

**Recency:** Current; represents cutting-edge multi-agent orchestration and persona-driven architecture patterns.

**Source:** [gridaco/grida/.agents/skills/sdk-seam/SKILL.md](https://github.com/gridaco/grida/blob/5fcea20837f696e6071b01d79e92ce72006d5891/.agents/skills/sdk-seam/SKILL.md) · 2522★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: sdk-seam
description: >
  Discipline for the seam between two SDKs (or two sides of one
  contract) that the same hand writes. The failure mode: "we own
  both sides" produces dirty contracts no foreign reviewer would
  accept. The exercise: pretend the other side is FFI, IPC, or a
  network protocol you cannot rewrite. Spawn an adversarial subagent
  profiled as the producer's maintainer; negotiate the change as a
  feature request, not a PR. Companion to $sdk-design.
  Language-agnostic — applies to a TS package + its consumer, a Rust
  crate + its WASM binding, two services sharing a wire format, or
  any other boundary the same author writes both ends of.
---

# sdk-seam

> Companion to [`sdk-design`](../sdk-design/SKILL.md). Read that
> first; its deciding table and disciplines are the foundation this
> skill builds on. Where `sdk-design` is about a single SDK's
> surface, this skill is about the **seam** — the joint between two
> SDKs (or two sides of one contract) — and what it takes to keep
> that joint clean when the same author writes both sides.

## The failure mode

When you control both sides of a boundary, you produce dirty
contracts — **simply because you c
```

</details>
