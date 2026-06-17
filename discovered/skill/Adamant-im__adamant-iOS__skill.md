---
name: Adamant-im__adamant-iOS__skill
source: https://github.com/Adamant-im/adamant-iOS/blob/7823857161c4d3e892bb6c8d8a2e9f1150a1b196/.ai/skills/code-style/SKILL.md
repo: Adamant-im/adamant-iOS
kind: skill
stars: 469
last_pushed: 2026-03-28T08:35:59Z
license: gpl-3.0
score: 8
domains: [ios, mobile-development, swift]
tags: [di-patterns, architectural-rules, code-quality]
curated: 2026-06-15
curated_by: config-scout
---

# Adamant-im/adamant-iOS — skill

**Why it's worth keeping:** It includes actionable instructions for service registration patterns and explicit behavioral rules for handling legacy code/migrations to prevent technical debt.

**Summary:** Provides specific architectural constraints for an iOS project, covering dependency injection via Swinject and protocol-level compatibility.

**Source credibility:** High; a well-starred repository (469 stars) indicating real-world production usage.

**Recency:** Current; updated within the last 3 months.

**Source:** [Adamant-im/adamant-iOS/.ai/skills/code-style/SKILL.md](https://github.com/Adamant-im/adamant-iOS/blob/7823857161c4d3e892bb6c8d8a2e9f1150a1b196/.ai/skills/code-style/SKILL.md) · 469★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: code-style
description: iOS platform rules, Swift conventions, dependency injection patterns, and code quality standards for ADAMANT iOS. Use when writing or reviewing code.
license: Apache-2.0
compatibility: Swift 5.9+, iOS 15.0+, UIKit, Swinject
metadata:
  project: adamant-ios
  domain: code-quality
---

# Code Style and Quality

Code style conventions, platform rules, and quality standards for ADAMANT iOS.

## iOS Platform and Swift Rules

- **Target iOS 15.0+** as specified in `Podfile` and package manifests
- **Use Swift 5.9+** language features as appropriate
- **Follow UIKit patterns**; this is not a SwiftUI project
- **Respect iOS lifecycle events** and state restoration
- **Handle memory warnings and background transitions** properly
- **Use `@MainActor`** or `DispatchQueue.main.async` for UI updates from background threads
- **Avoid force unwrapping (`!`)** except in truly safe scenarios; prefer optional binding or guard statements
- **Use Swift's type safety and value semantics** where appropriate

## Dependency Injection Rules

- **All services must be registered** in appropriate assembly files (`Adamant/App/DI/*`, module-specific assemblies)
- **Use protocol
```

</details>
