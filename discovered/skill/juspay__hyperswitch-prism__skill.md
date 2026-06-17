---
name: juspay__hyperswitch-prism__skill
source: https://github.com/juspay/hyperswitch-prism/blob/a4aae87dd98b852d995234f103e5a9d47ebbcd71/.skills/new-connector/SKILL.md
repo: juspay/hyperswitch-prism
kind: skill
stars: 1421
last_pushed: 2026-06-16T05:29:54Z
license: apache-2.0
score: 9
domains: [backend-api, rust, agents-ai]
tags: [orchestrator, subagent-pattern, workflow-automation, industrial-grade]
curated: 2026-06-16
curated_by: config-scout
---

# juspay/hyperswitch-prism — skill

**Why it's worth keeping:** Uses a strict 'Orchestrator/Subagent' pattern with explicit 'Gate' logic (hard stops) to prevent hallucination. The sequential, flow-based delegation ensures every architectural layer is validated before proceeding.

**Summary:** A high-sophistication orchestrator skill that manages complex Rust module creation via specialized subagents.

**Source credibility:** High; comes from an established, well-starred open-source payment infrastructure project (Hyperswitch).

**Recency:** Highly current; demonstrates advanced multi-agent coordination techniques relevant to modern AI coding workflows.

**Source:** [juspay/hyperswitch-prism/.skills/new-connector/SKILL.md](https://github.com/juspay/hyperswitch-prism/blob/a4aae87dd98b852d995234f103e5a9d47ebbcd71/.skills/new-connector/SKILL.md) · 1421★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: new-connector
description: >
  Implements a new payment connector from scratch in the connector-service (UCS) Rust codebase.
  Creates connector foundation and implements all 6 core payment flows (Authorize, PSync, Capture,
  Refund, RSync, Void). Use when integrating a new payment gateway that does not yet exist.
  Requires a technical specification at grace/rulesbook/codegen/references/{connector_name}/technical_specification.md.
license: Apache-2.0
compatibility: Requires Rust toolchain with cargo. Linux or macOS.
metadata:
  author: parallal
  version: "2.0"
  domain: payment-connectors
---

# New Connector Implementation

## Overview

This skill produces a complete payment connector in the UCS Rust codebase.

**MANDATORY SUBAGENT DELEGATION: You are the orchestrator. You MUST delegate every step
to a subagent using the prompts in `references/subagent-prompts.md`. Do NOT implement
code, run tests, or review quality yourself. Spawn subagents and coordinate their outputs.**

**Output:**
- Main connector file with macro-based flow implementations
- Transformers module with request/response types and conversions
- Registration in the connector registry
- All 6 core flows
```

</details>
