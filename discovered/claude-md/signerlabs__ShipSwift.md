---
name: signerlabs__ShipSwift
source: https://github.com/signerlabs/ShipSwift/blob/0877b3af0136329e9c9ef4c44bdc5e19e115534f/CLAUDE.md
repo: signerlabs/ShipSwift
kind: claude-md
stars: 2175
last_pushed: 2026-06-08T04:36:13Z
license: mit
score: 9
domains: [ios, swiftui, mobile-development]
tags: [architecture-enforcement, naming-conventions, modularization]
curated: 2026-06-14
curated_by: config-scout
---

# signerlabs/ShipSwift — claude-md

**Why it's worth keeping:** The explicit dependency hierarchy prevents spaghetti code, while the specific platform-suffix rules provide actionable instructions for maintaining Xcode build phases.

**Summary:** Defines strict architectural boundaries and naming conventions for a modular SwiftUI component library.

**Source credibility:** High; 2k+ stars and recent activity indicate a well-maintained, community-vetted project.

**Recency:** Current; aligned with modern SwiftUI development workflows and multi-platform iOS/macOS support.

**Source:** [signerlabs/ShipSwift/CLAUDE.md](https://github.com/signerlabs/ShipSwift/blob/0877b3af0136329e9c9ef4c44bdc5e19e115534f/CLAUDE.md) · 2175★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview
- ShipSwift iOS component template library (public repo)

## Directory Structure
- Reusable components live under `ShipSwift/SWPackage/` in five directories:
  - `SWAnimation/` — Self-contained animation components (each works independently, may depend on SWUtil only)
  - `SWChart/` — Self-contained chart components (each works independently, may depend on SWUtil only)
  - `SWComponent/` — Self-contained UI components organized by category:
    - `Display/` — Display components (FloatingLabels, MarkdownText, ScrollingFAQ, RotatingQuote, BulletPointText, GradientDivider, Label, OnboardingView, OrderView, RootTabView)
    - `Feedback/` — Feedback components (Alert, Loading, ThinkingIndicator)
    - `Input/` — Input components (TabButton, Stepper, AddSheet, SearchBar)
  - `SWModule/` — Multi-file frameworks (SWAuth, SWCamera, SWPaywall, SWChat, SWSetting, SWSubjectLifting, SWTikTokTracking)
  - `SWUtil/` — Shared utilities (no dependencies on other SWPackage directories)
- Showcase app views live under `ShipSwift/View/` (HomeView, ChatView, ComponentView, ProPaywallView, RootTabView, SettingView, ShipSwiftAuthView)
- App services live under `ShipSwift/
```

</details>
