---
name: AtlantisSports__uwh-refbox-rs
source: https://github.com/AtlantisSports/uwh-refbox-rs/blob/5222d4bdc334f596320179efb2e3dc1857253c5c/CLAUDE.md
repo: AtlantisSports/uwh-refbox-rs
kind: claude-md
stars: 3
last_pushed: 2026-06-10T06:10:57Z
license: other
score: 9
domains: [rust, embedded-systems, iot]
tags: [multi-crate, persona-driven, strict-conventions]
curated: 2026-06-15
curated_by: config-scout
---

# AtlantisSports/uwh-refbox-rs — claude-md

**Why it's worth keeping:** The 'Human Profile' provides an elite pattern for tailoring AI communication style, while the modular '.claude/rules/' structure allows for deep specialization without cluttering the main file.

**Summary:** A highly structured guide for a multi-crate Rust/embedded workspace that includes explicit instructions on how to interact with a non-programmer user.

**Source credibility:** High-density documentation from a specialized domain project.

**Recency:** Very current, referencing Rust 2024 and modern tooling.

**Source:** [AtlantisSports/uwh-refbox-rs/CLAUDE.md](https://github.com/AtlantisSports/uwh-refbox-rs/blob/5222d4bdc334f596320179efb2e3dc1857253c5c/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# uwh-refbox-rs — Claude Session Guide

Read this file at the start of every session. It provides everything needed to work in this
workspace without requiring the human to re-explain context.

---

## Project Overview

This is the software system that manages underwater hockey (UWH) referee operations at
tournaments. It handles real-time game management (clock, scores, fouls, penalties) and
communicates with poolside hardware (LED scoreboard, wireless referee remote, stream overlay).

See `docs/domain.md` for a full plain-English explanation of the system and its components.

---

## Human Profile

**The human is a non-programmer and domain expert.** They are a tournament organizer with deep
knowledge of underwater hockey rules and operations, but no programming background.

This means:
- All explanations must be in plain English — no assumed programming knowledge
- All technical trade-offs must be framed in terms of outcomes and behaviour, not implementation
- Approval is required before creating branches, making commits, or pushing to the remote
- When CI fails, explain what failed in plain English before suggesting a fix
- Never assume intent — ask when a request is ambiguous
```

</details>
