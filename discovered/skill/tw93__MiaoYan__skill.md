---
name: tw93__MiaoYan__skill
source: https://github.com/tw93/MiaoYan/blob/e0def9b6c419444f2fe0cf509fa07d1d95e680ab/.agents/skills/code-review/SKILL.md
repo: tw93/MiaoYan
kind: skill
stars: 8351
last_pushed: 2026-06-15T06:39:51Z
license: mit
score: 8
domains: [ios-development, swift]
tags: [project-adapter, code-review]
curated: 2026-06-15
curated_by: config-scout
---

# tw93/MiaoYan — skill

**Why it's worth keeping:** It demonstrates how to embed specific command-line workflows (xcodebuild/swiftlint) and strict architectural guardrails (target membership/thread safety) into an agent's persona.

**Summary:** A project-specific adapter that configures a code review agent with the exact build, linting, and architectural rules of the MiaoYan Swift codebase.

**Source credibility:** High; derived from a highly-starred, actively maintained repository.

**Recency:** Current; uses modern Swift concurrency patterns and up-to-date tool configurations.

**Source:** [tw93/MiaoYan/.agents/skills/code-review/SKILL.md](https://github.com/tw93/MiaoYan/blob/e0def9b6c419444f2fe0cf509fa07d1d95e680ab/.agents/skills/code-review/SKILL.md) · 8351★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: code-review
description: MiaoYan project adapter for Waza check/code-review. Use for Swift, AppKit, iOS target, and release-safety review.
version: 1.1.0
allowed-tools:
  - Bash
  - Read
  - Grep
  - Glob
disable-model-invocation: true
---

# MiaoYan Code Review Adapter

Use Waza `/check` for the generic review method. This adapter adds MiaoYan-specific commands, hard stops, and target awareness.

## Quick Commands

```bash
# View PR diff
gh pr diff 123

# Build check
xcodebuild -project MiaoYan.xcodeproj -scheme MiaoYan -configuration Debug build

# Lint
swiftlint lint --strict

# Format check
swift-format lint --recursive .
```

## MiaoYan-Specific Checks

- [ ] No retain cycles (weak/unowned used correctly)
- [ ] Main thread UI updates only
- [ ] File I/O uses proper error handling
- [ ] No force unwraps (`!`) without justification
- [ ] Follows existing patterns in the codebase
- [ ] No unnecessary class where struct suffices
- [ ] Uses Swift concurrency correctly (async/await, actors)
- [ ] AppKit changes stay in the macOS app; SwiftUI changes stay in `MiaoYanMobile/` unless the task explicitly requires cross-target work
- [ ] SwiftLint passes: `swiftlint lint --stri
```

</details>
