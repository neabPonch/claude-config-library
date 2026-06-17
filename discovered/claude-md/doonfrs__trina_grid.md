---
name: doonfrs__trina_grid
source: https://github.com/doonfrs/trina_grid/blob/791d0b2c8642b971ee90105473ccff78c922cef8/CLAUDE.md
repo: doonfrs/trina_grid
kind: claude-md
stars: 157
last_pushed: 2026-06-08T22:36:23Z
license: mit
score: 9
domains: [flutter, dart, ui-components]
tags: [architecture-mapping, workflow-enforcement, testing-patterns]
curated: 2026-06-14
curated_by: config-scout
---

# doonfrs/trina_grid — claude-md

**Why it's worth keeping:** The specific 'Workflow Rules' for running analysis/format prevent linting regressions, while the hierarchical breakdown of the source tree allows Claude to navigate deep file structures without guessing.

**Summary:** This config provides a high-density architectural map of a complex component library and enforces strict quality control steps.

**Source credibility:** Strong; 157 stars and very recent updates indicate a stable, real-world library.

**Recency:** Current; follows modern agentic workflow patterns including linting/formatting enforcement.

**Source:** [doonfrs/trina_grid/CLAUDE.md](https://github.com/doonfrs/trina_grid/blob/791d0b2c8642b971ee90105473ccff78c922cef8/CLAUDE.md) · 157★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

TrinaGrid is a Flutter package providing a keyboard-navigable data grid widget. It supports multiple column types (text, number, date, time, boolean, select, currency, percentage, custom), in-place editing, filtering, sorting, pagination, and export (CSV, JSON, PDF). Works on web, desktop, and mobile. Fork/continuation of the discontinued PlutoGrid.

## Common Commands

```bash
flutter pub get                      # Install dependencies
flutter test                         # Run all tests
flutter test test/path/to_test.dart  # Run a single test file
flutter test --coverage              # Run tests with coverage
dart analyze                         # Check for analysis errors
dart format .                        # Format all code
dart fix --apply                     # Apply automated fixes
```

## Workflow Rules

- **IMPORTANT: After finishing any code changes**, you MUST run `dart format` on the edited files and then run `dart analyze` to check for errors. Fix any issues found before considering the task done. Never skip this step.
- If an API or
```

</details>
