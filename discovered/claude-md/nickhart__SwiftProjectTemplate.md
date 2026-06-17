---
name: nickhart__SwiftProjectTemplate
source: https://github.com/nickhart/SwiftProjectTemplate/blob/52b622e5c6c606ca7b01eb023f59aa613bfd9c77/CLAUDE.md
repo: nickhart/SwiftProjectTemplate
kind: claude-md
stars: 3
last_pushed: 2025-10-18T05:53:41Z
license: mit
score: 9
domains: [ios-development, mobile-app, automation]
tags: [swift, xcodegen, shell-scripting]
curated: 2026-06-16
curated_by: config-scout
---

# nickhart/SwiftProjectTemplate — claude-md

**Why it's worth keeping:** It utilizes a 'Command-First' approach by mapping every developer action to specific shell scripts with detailed flag documentation. It also establishes crucial architectural constraints, such as instructing the AI to use xcodegen rather than manual Xcode project manipulation.

**Summary:** This file provides exhaustive guidance on a script-driven development workflow using XcodeGen. It defines clear paths for project generation (ADOPT vs GENERATE) and strict quality enforcement through a preflight script.

**Source credibility:** 3 stars indicates a specialized niche template rather than a major framework, but the content is highly professional.

**Recency:** 8 months old; well-aligned with current iOS development and automation standards.

**Source:** [nickhart/SwiftProjectTemplate/CLAUDE.md](https://github.com/nickhart/SwiftProjectTemplate/blob/52b622e5c6c606ca7b01eb023f59aa613bfd9c77/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### Essential Commands
- `./scripts/setup.sh` - One-time project setup: installs dependencies, generates project, configures simulators
- `./scripts/build.sh` - Build the app (add `--device` for device builds, `--release` for Release config)
- `./scripts/test.sh` - Run unit tests (add `--ui` for UI tests, `--all` for both, `--release` for Release config)
- `./scripts/lint.sh` - Check code style with SwiftLint (add `--fix` for auto-fix, `--strict` for warnings as errors)
- `./scripts/format.sh` - Check code formatting with SwiftFormat (add `--fix` for auto-fix)
- `./scripts/preflight.sh` - Complete local CI check: fixes formatting, runs linting, builds, and tests
- `xcodegen` - Regenerate Xcode project from project.yml (required after adding/removing files or changing project structure)

### Simulator Management
- `./scripts/simulator.sh list` - Show available simulators
- `./scripts/simulator.sh config-tests "device-name"` - Configure simulator for unit tests
- `./scripts/simulator.sh config-ui-tests "device-name"` - Configure simulator for U
```

</details>
