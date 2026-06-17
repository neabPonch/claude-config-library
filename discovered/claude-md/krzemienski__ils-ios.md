---
name: krzemienski__ils-ios
source: https://github.com/krzemienski/ils-ios/blob/2c3deb83e9d2acdaffbb2a33d883317460d8add4/CLAUDE.md
repo: krzemienski/ils-ios
kind: claude-md
stars: 1
last_pushed: 2026-03-22T19:45:01Z
license: mit
score: 9
domains: [ios, macos, swift, backend-api]
tags: [monorepo, build-verification, pitfalls, apple-ecosystem]
curated: 2026-06-16
curated_by: config-scout
---

# krzemienski/ils-ios — claude-md

**Why it's worth keeping:** The 'Common Pitfalls' section provides extremely valuable, specific technical edge cases (e.g., Crypto vs CryptoKit), and the use of a dedicated Simulator UDID is a brilliant technique for multi-session environment control.

**Summary:** A high-density instruction set for a Swift monorepo that combines environmental constraints with a rigorous build-verification workflow.

**Source credibility:** High; comes from an active native iOS/macOS project with recent commits.

**Recency:** Very current, referencing iOS 18.6 and modern Swift development patterns.

**Source:** [krzemienski/ils-ios/CLAUDE.md](https://github.com/krzemienski/ils-ios/blob/2c3deb83e9d2acdaffbb2a33d883317460d8add4/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ILS iOS/macOS App — Project Instructions

## Project Context

This is a **Swift iOS/macOS monorepo** for ILS (Intelligent Local Server), a native client for Claude Code.

**Key Paths:**
- `ILSApp/ILSApp/` — iOS app source (SwiftUI)
- `ILSApp/ILSMacApp/` — macOS app source (SwiftUI)
- `ILSApp/ILSApp.xcodeproj` — Xcode project (also `project.yml` for XcodeGen)
- `Sources/ILSBackend/` — Vapor backend (Swift)
- `Sources/ILSShared/` — Shared models between iOS and backend
- `scripts/` — setup.sh, install-backend-service.sh, run_regression_tests.sh
- `.claude/plan/` — Planning documents
- `.sop/` — Structured operating procedures and specs
- `AppStoreMetadata/` — Screenshots and metadata for App Store submission

**Bundle ID:** `com.ils.app` (iOS), `com.ils.mac` (macOS)
**URL Scheme:** `ils://` (registered in Info.plist)
**Backend Port:** 9999 (avoid 8080 — used by ralph-mobile)
**API Prefix:** `/api/v1` (added by APIClient.swift)

**Backend Controllers:** Sessions, Projects, Chat, Skills, MCP, Plugins, Config, Stats, Themes, System, Teams, Tunnel

**Build Commands:**
```bash
# iOS
xcodebuild -project ILSApp/ILSApp.xcodeproj -scheme ILSApp -destination 'id=50523130-57AA-48B0-ABD0-4D59C
```

</details>
