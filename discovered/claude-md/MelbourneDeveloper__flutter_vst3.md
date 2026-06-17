---
name: MelbourneDeveloper__flutter_vst3
source: https://github.com/MelbourneDeveloper/flutter_vst3/blob/39d5e4290cb6ee3e9f0cc2b12ae52d5225e02c6c/CLAUDE.md
repo: MelbourneDeveloper/flutter_vst3
kind: claude-md
stars: 47
last_pushed: 2026-06-01T17:49:24Z
license: unknown
score: 9
domains: [audio-engineering, dart-flutter, systems-programming]
tags: [strict-coding-standards, vst3, ffi, functional-programming]
curated: 2026-06-15
curated_by: config-scout
---

# MelbourneDeveloper/flutter_vst3 — claude-md

**Why it's worth keeping:** The 'Fail Hard' and 'No Placeholders' rules are elite guardrails against AI-generated technical debt; the explicit file/function length limits provide clear, actionable maintainability metrics.

**Summary:** Defines extreme coding standards and architectural constraints for a complex Dart/C++ audio toolkit.

**Source credibility:** High; highly specialized, professional-grade domain expertise in audio processing.

**Recency:** Current; includes specific requirements for modern Dart patterns like pattern matching.

**Source:** [MelbourneDeveloper/flutter_vst3/CLAUDE.md](https://github.com/MelbourneDeveloper/flutter_vst3/blob/39d5e4290cb6ee3e9f0cc2b12ae52d5225e02c6c/CLAUDE.md) · 47★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Code Rules
- NO PLACEHOLDERS. NO FALLBACKS. FAIL HARD!!! If the code is not implemented, THROW AN ERROR!!! Fail LOUDLY by throwing an exception.
- NO DUPLICATION. Move files, code elements instead of copying them. Search for elements before adding them.
- FP style. No interfaces, classes, or mutable state. Pure functions with no side effects.
- Tests must FAIL HARD. Don't add allowances and print warnings. Just FAIL!
- Keep functions under 20 lines long.
- Do not use Git commands unless explicitly requested
- Keep files under 400 LOC, even tests

## Dart Rules
- NEVER use the late keyword
- Document all public functions with Dart /// doc, especially the important ones
- Don't use if statements. Use pattern matching or ternaries instead.
- Only native machine code. No AOT or Dart runtime!


## Project Overview

This a Steinberg VST® 3 toolkit for Dart and Flutter. Use this toolkit to implement VST® plugins and VST® hosts. This toolkit enables anyone to create VST® 3 plugins with pure Dart and Flutter.

*VST® is a trademark of Steinberg Media Technologies GmbH.*

Th
```

</details>
