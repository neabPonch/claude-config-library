---
name: Iron-Ham__XcodePreviews__skill
source: https://github.com/Iron-Ham/XcodePreviews/blob/9f291f62be01442c2c27f5ffd4de71bcb3feb23f/.cursor/skills/preview/SKILL.md
repo: Iron-Ham/XcodePreviews
kind: skill
stars: 142
last_pushed: 2026-05-11T14:39:53Z
license: mit
score: 8
domains: [ios-development, mobile-ui, cli-tools]
tags: [swiftui, xcode, visual-regression, simulator]
curated: 2026-06-16
curated_by: config-scout
---

# Iron-Ham/XcodePreviews — skill

**Why it's worth keeping:** It provides a structured 'Workflow' pattern (Build -> Capture -> Read -> Report) that teaches the agent how to perform visual regression testing. It also effectively abstracts project-specific complexities like SPM vs Xcode projects.

**Summary:** Enables an agent to compile SwiftUI code and capture screenshots for automated visual analysis and UI verification.

**Source credibility:** Decent popularity for a niche utility with very active maintenance.

**Recency:** Highly current, updated within the last month.

**Source:** [Iron-Ham/XcodePreviews/.cursor/skills/preview/SKILL.md](https://github.com/Iron-Ham/XcodePreviews/blob/9f291f62be01442c2c27f5ffd4de71bcb3feb23f/.cursor/skills/preview/SKILL.md) · 142★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: preview-build
description: Build and capture SwiftUI previews for visual analysis. Use when the user asks to preview a SwiftUI view, capture a simulator screenshot, or visually inspect iOS UI components. Supports Xcode projects, SPM packages, and standalone Swift files.
---

# Xcode Preview Capture Skill

Build SwiftUI views and capture screenshots of their rendered output for visual analysis.

## Installation Path

Scripts are located at `${PREVIEW_BUILD_PATH:-$HOME/XcodePreviews}/scripts/`

> **Compatibility:** If `~/XcodePreviews` doesn't exist, fall back to `~/Claude-XcodePreviews` (legacy name). The `PREVIEW_BUILD_PATH` environment variable overrides both.

## Available Commands

### Unified Preview (Recommended)

Auto-detects project type and uses the best approach:

```bash
"${PREVIEW_BUILD_PATH:-$HOME/XcodePreviews}"/scripts/preview \
  <path-to-file.swift> \
  --output /tmp/preview.png
```

### Quick Capture (Current Simulator)

```bash
"${PREVIEW_BUILD_PATH:-$HOME/XcodePreviews}"/scripts/capture-simulator.sh \
  --output /tmp/preview-capture.png
```

### Xcode Project with #Preview

Fast builds by injecting a minimal PreviewHost target (handled automatically by
```

</details>
