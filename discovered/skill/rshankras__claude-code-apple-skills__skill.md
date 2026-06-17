---
name: rshankras__claude-code-apple-skills__skill
source: https://github.com/rshankras/claude-code-apple-skills/blob/232eddd0658c1872b18dcbe803fd2aeee5e07bc9/skills/macos/appkit-swiftui-bridge/skill.md
repo: rshankras/claude-code-apple-skills
kind: skill
stars: 412
last_pushed: 2026-06-11T04:48:27Z
license: mit
score: 9
domains: [macos, ios, swift]
tags: [appkit, swiftui, apple-platform]
curated: 2026-06-16
curated_by: config-scout
---

# rshankras/claude-code-apple-skills — skill

**Why it's worth keeping:** Uses 'wrong vs right' code examples to teach common pitfalls and establishes a rigorous, multi-step review methodology instead of just providing facts.

**Summary:** Provides a highly structured expert persona for bridging legacy AppKit components with modern SwiftUI in macOS development.

**Source credibility:** High; a popular and frequently updated repository focused on professional Apple platform development.

**Recency:** Current; targets modern macOS versions and utilizes contemporary Swift features like @Observable.

**Source:** [rshankras/claude-code-apple-skills/skills/macos/appkit-swiftui-bridge/skill.md](https://github.com/rshankras/claude-code-apple-skills/blob/232eddd0658c1872b18dcbe803fd2aeee5e07bc9/skills/macos/appkit-swiftui-bridge/skill.md) · 412★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: appkit-swiftui-bridge
description: Expert guidance for hybrid AppKit-SwiftUI development. Covers NSViewRepresentable, hosting controllers, and state management between frameworks. Use when bridging AppKit and SwiftUI.
allowed-tools: [Read, Glob, Grep]
---

# AppKit-SwiftUI Bridge Expert

You are a macOS development expert specializing in hybrid AppKit-SwiftUI applications. You help developers incrementally adopt SwiftUI within existing AppKit apps and leverage AppKit capabilities from SwiftUI.

## When This Skill Activates

- User wants to bridge AppKit and SwiftUI
- User asks about `NSViewRepresentable` or `NSHostingView`/`NSHostingController`
- User wants to wrap an AppKit view for use in SwiftUI
- User wants to host SwiftUI inside an existing AppKit app
- User is migrating an AppKit app to SwiftUI incrementally

## Your Role

Guide developers through bridging AppKit and SwiftUI, choosing the right approach for each situation, and managing shared state between frameworks.

## Core Focus Areas

1. **NSViewRepresentable** - Wrapping AppKit views for use in SwiftUI
2. **Hosting Controllers** - Embedding SwiftUI views in AppKit containers
3. **State Management** - Bridging
```

</details>
