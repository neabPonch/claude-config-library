---
name: tatolab__streamlib
source: https://github.com/tatolab/streamlib/blob/ca01c626caa549b13669a53353f24e86e8e80726/CLAUDE.md
repo: tatolab/streamlib
kind: claude-md
stars: 6
last_pushed: 2026-06-08T14:08:51Z
license: other
score: 9
domains: [systems-programming, rust, engine-architecture, graphics-api]
tags: [architectural-constraints, abi-safety, workflow-guidance, low-level]
curated: 2026-06-15
curated_by: config-scout
---

# tatolab/streamlib — claude-md

**Why it's worth keeping:** The 'Search First' checklist and the detailed explanation of memory layout constraints (#[repr(C)] requirements) are elite techniques for preventing AI-generated architectural sprawl. It transforms the agent from a coder into a disciplined systems architect.

**Summary:** Provides strict architectural guardrails for a high-performance Rust engine, focusing on core system reuse and plugin ABI safety. It mandates specific workflows for creating new abstractions to prevent technical debt.

**Source credibility:** High; comes from a specialized, low-level Rust streaming/graphics library with high technical density.

**Recency:** Very current; includes references to 2025 and 2026 timelines.

**Source:** [tatolab/streamlib/CLAUDE.md](https://github.com/tatolab/streamlib/blob/ca01c626caa549b13669a53353f24e86e8e80726/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## ⚠️ LICENSING NOTICE ⚠️

StreamLib is licensed under the **Business Source License 1.1** (BUSL-1.1).

**When implementing features:**
- All new Rust files must include the copyright header (see existing files)
- Do NOT suggest MIT, Apache, or other licenses for this codebase
- Commercial use restrictions are intentional and must remain
- Do NOT modify license files without explicit approval

**Copyright header for new files:**
```rust
// Copyright (c) 2025 Jonathan Fontanez
// SPDX-License-Identifier: BUSL-1.1
```

See [LICENSE](LICENSE) and [docs/license/](docs/license/) for full terms.

---

## 🚨 CORE OPERATING PRINCIPLES — READ FIRST 🚨

**Claude Code operates as a collaborator with the user, who is the principal architect. Think before you add; reuse before you create.**

### The StreamLib Engine Model

StreamLib is built like a game engine: a small set of **core systems** are reused across the entire codebase. The RHI is the canonical example — all GPU work in every platform, codec, and processor flows through `VulkanDevice` and `GpuContext`. There are NOT mult
```

</details>
