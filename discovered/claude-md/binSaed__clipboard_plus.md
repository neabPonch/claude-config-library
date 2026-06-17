---
name: binSaed__clipboard_plus
source: https://github.com/binSaed/clipboard_plus/blob/fb9c2267b492be47a99addc20e1a352ed6231e17/CLAUDE.md
repo: binSaed/clipboard_plus
kind: claude-md
stars: 0
last_pushed: 2026-01-25T04:01:20Z
license: mit
score: 7
domains: [mobile-dev, flutter, android]
tags: [testing, flutter, unit-tests]
curated: 2026-06-16
curated_by: config-scout
---

# binSaed/clipboard_plus — claude-md

**Why it's worth keeping:** Provides highly actionable shell commands and specific guidance on mocking requirements and edge-case coverage.

**Summary:** Defines rigorous testing workflows including exact command-line instructions for both Flutter and Android native layers.

**Source credibility:** Low social proof; single contributor repository with 0 stars.

**Recency:** Current; last pushed 5 months ago.

**Source:** [binSaed/clipboard_plus/CLAUDE.md](https://github.com/binSaed/clipboard_plus/blob/fb9c2267b492be47a99addc20e1a352ed6231e17/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project Instructions

## Testing Requirements

**IMPORTANT:** For every task that modifies code:

1. **Run existing tests** before and after making changes
2. **Add new tests** for any new functionality
3. **Update existing tests** if behavior changes
4. **Ensure all tests pass** before considering the task complete

### Test Commands

```bash
# Run all Flutter tests
flutter test

# Run tests with coverage
flutter test --coverage

# Run Android unit tests (from example/android/)
./gradlew testDebugUnitTest
```

### Test Structure

- `test/` - Flutter unit tests and widget tests
- `android/src/test/` - Android Kotlin unit tests
- `example/test/` - Example app tests (if applicable)

### Test Expectations

- Unit tests for all public API methods in `ClipboardPlus`
- Mock platform channels for testing native calls
- Test edge cases (null values, empty strings, etc.)
- Test `ClipboardContentType` data class
```

</details>
