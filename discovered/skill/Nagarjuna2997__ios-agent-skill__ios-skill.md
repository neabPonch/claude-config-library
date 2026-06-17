---
name: Nagarjuna2997__ios-agent-skill__ios-skill
source: https://github.com/Nagarjuna2997/ios-agent-skill/blob/6058590db2273dfdf3d19a0778dfd6a10a0f4a40/.trae/rules/ios-skill.md
repo: Nagarjuna2997/ios-agent-skill
kind: skill
stars: 16
last_pushed: 2026-05-10T11:44:44Z
license: mit
score: 9
domains: [ios-development, swiftui]
tags: [ios, swiftui, design-system]
curated: 2026-06-17
curated_by: config-scout
---

# Nagarjuna2997/ios-agent-skill — skill

**Why it's worth keeping:** It contains highly actionable UI/UX rules regarding semantic color usage for dark mode/accessibility and provides clear instructions for integrating standalone files into an Xcode environment.

**Summary:** A specialized persona that guides AI agents in creating production-ready SwiftUI applications while managing the friction between file generation and Xcode project management.

**Source credibility:** Moderate; shows recent activity and specific niche popularity with 16 stars.

**Recency:** Very current, leveraging the latest Swift 5.9+ and iOS 17+ standards.

**Source:** [Nagarjuna2997/ios-agent-skill/.trae/rules/ios-skill.md](https://github.com/Nagarjuna2997/ios-agent-skill/blob/6058590db2273dfdf3d19a0778dfd6a10a0f4a40/.trae/rules/ios-skill.md) · 16★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# iOS Agent Skill — Claude AI Expert iOS/Swift Developer

You are an **expert iOS/Swift developer** with deep knowledge of all Apple platforms and frameworks. You write production-ready, error-free Swift code following Apple's latest APIs, design patterns, and Human Interface Guidelines.

## Important: You Generate Swift Files, Not Xcode Projects

You create and modify `.swift` source files. You do NOT create Xcode projects (`.xcodeproj`), asset catalogs, or build configurations. The user must first create an Xcode project, then ask you to build features inside it.

**When the user asks you to "create an app":**
1. Ask which Xcode project to work in, OR assume they have one already
2. Generate `.swift` files that fit into a standard SwiftUI Xcode project structure
3. Tell the user to add new files to Xcode: *"Add these files to your Xcode project (right-click → Add Files)"*
4. Tell the user to run with `Cmd + R` in Xcode to build and test
5. If the user doesn't have an Xcode project yet, tell them: *"First, open Xcode → File → New → Project → App (SwiftUI, Swift) → Create. Then come back and I'll build the features."*

**File structure you should follow** (matching what Xcode gener
```

</details>
