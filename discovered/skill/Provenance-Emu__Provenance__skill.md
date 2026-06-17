---
name: Provenance-Emu__Provenance__skill
source: https://github.com/Provenance-Emu/Provenance/blob/c3d001a12c8788aeb8e2e8246d1d3b6262bbce62/.agents/skills/swiftdata-pro/SKILL.md
repo: Provenance-Emu/Provenance
kind: skill
stars: 6331
last_pushed: 2026-06-09T13:56:33Z
license: other
score: 9
domains: [ios-development, swift]
tags: [swiftdata, ios, code-review]
curated: 2026-06-15
curated_by: config-scout
---

# Provenance-Emu/Provenance — skill

**Why it's worth keeping:** The 'load only relevant references' pattern is an elite way to manage context; the specific 'before/after' examples provide perfect structural templates for agent outputs.

**Summary:** A highly specialized tool for SwiftData development that utilizes a modular, reference-based review process to ensure architectural correctness.

**Source credibility:** Very high: Authored by Paul Hudson, one of the most respected authorities in iOS development.

**Recency:** Current: specifically targets Swift 6 and modern iOS capabilities.

**Source:** [Provenance-Emu/Provenance/.agents/skills/swiftdata-pro/SKILL.md](https://github.com/Provenance-Emu/Provenance/blob/c3d001a12c8788aeb8e2e8246d1d3b6262bbce62/.agents/skills/swiftdata-pro/SKILL.md) · 6331★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: swiftdata-pro
description: Writes, reviews, and improves SwiftData code using modern APIs and best practices. Use when reading, writing, or reviewing projects that use SwiftData.
license: MIT
metadata:
  author: Paul Hudson
  version: "1.0"
---

Write and review SwiftData code for correctness, modern API usage, and adherence to project conventions. Report only genuine problems - do not nitpick or invent issues.

Review process:

1. Check for core SwiftData issues using `references/core-rules.md`.
1. Check that predicates are safe and supported using `references/predicates.md`.
1. If the project uses CloudKit, check for CloudKit-specific constraints using `references/cloudkit.md`.
1. If the project targets iOS 18+, check for indexing opportunities using `references/indexing.md`.
1. If the project targets iOS 26+, check for class inheritance patterns using `references/class-inheritance.md`.

If doing partial work, load only the relevant reference files.


## Core Instructions

- Target Swift 6.2 or later, using modern Swift concurrency.
- The user strongly prefers to use SwiftData across the board. Do not suggest Core Data functionality unless it is a feature that cannot be
```

</details>
