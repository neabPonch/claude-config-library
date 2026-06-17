---
name: openwebf__webf__claude
source: https://github.com/openwebf/webf/blob/c091d3349168947f590dc00efa8bdd83c4c98402/webf/CLAUDE.md
repo: openwebf/webf
kind: claude-md
stars: 2476
last_pushed: 2026-06-11T16:09:28Z
license: gpl-3.0
score: 8
domains: [mobile-dev, flutter-dart, testing]
tags: [dart, flutter, unit-testing, integration-testing]
curated: 2026-06-15
curated_by: config-scout
---

# openwebf/webf — claude-md

**Why it's worth keeping:** Includes high-value boilerplate for test setup/teardown and explicit strategies for verifying rendering changes without full app execution.

**Summary:** Provides detailed technical instructions for Dart/Flutter development specifically tailored to the WebF framework's unique testing requirements.

**Source credibility:** High; a popular open-source project with significant star count and recent maintenance.

**Recency:** Highly current, with very recent activity.

**Source:** [openwebf/webf/webf/CLAUDE.md](https://github.com/openwebf/webf/blob/c091d3349168947f590dc00efa8bdd83c4c98402/webf/CLAUDE.md) · 2476★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Dart/Flutter Development Guide (webf/)

This guide covers Dart/Flutter development in the `webf/` directory, which implements DOM/CSS and layout/painting on top of Flutter.

## Development Workflow
- No build needed for Dart-only changes
- Use widget unit tests to verify rendering changes: `cd webf && flutter test test/src/rendering/`
- Use integration tests for end-to-end verification: `cd webf && flutter test integration_test/`

## Dart Code Style
- Follow rules in webf/analysis_options.yaml
- Use single quotes for strings
- File names must use snake_case
- Class names must use PascalCase
- Variables/functions use camelCase
- Prefer final fields when applicable
- Lines should be max 120 characters

## Lint and Format Commands
- Lint: `npm run lint` (runs flutter analyze in webf directory)
- Format: `npm run format` (formats with 120 char line length)

## Dart/Flutter Testing
- Run Flutter dart tests: `cd webf && flutter test`
- Run a single Flutter test: `cd webf && flutter test test/path/to/test_file.dart`
- Run widget unit tests: `cd webf && flutter test test/src/rendering/`
- Run integration tests: `cd webf && flutter test integration_test/`
- See Unit Tests (webf/test) sect
```

</details>
