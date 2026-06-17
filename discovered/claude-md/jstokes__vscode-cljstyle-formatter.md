---
name: jstokes__vscode-cljstyle-formatter
source: https://github.com/jstokes/vscode-cljstyle-formatter/blob/50c5c0ca15106db649cd9fdd8f07af8314470f92/CLAUDE.md
repo: jstokes/vscode-cljstyle-formatter
kind: claude-md
stars: 0
last_pushed: 2025-07-08T20:41:34Z
license: mit
score: 9
domains: [vscode-extensions, cli-tools]
tags: [architecture, implementation-logic, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# jstokes/vscode-cljstyle-formatter — claude-md

**Why it's worth keeping:** It includes 'Lessons Learned' to transmit developer philosophy and specific algorithmic strategies (like the smart expansion logic) directly to the AI. This ensures future features align with the project's technical standards and edge-case handling requirements.

**Summary:** This file provides deep architectural insight and implementation logic for a VSCode extension, covering both standard commands and complex algorithm strategies.

**Source credibility:** Single-author open-source tool with highly specialized, high-quality technical documentation.

**Recency:** Current; reflects modern TypeScript and VSCode API patterns.

**Source:** [jstokes/vscode-cljstyle-formatter/CLAUDE.md](https://github.com/jstokes/vscode-cljstyle-formatter/blob/50c5c0ca15106db649cd9fdd8f07af8314470f92/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a VSCode extension that formats Clojure code using the `cljstyle` formatter. The extension provides document and range formatting for Clojure files (`.clj`, `.cljs`, `.cljc`, `.edn`, `.fiddle`).

## Development Commands

- **Build**: `npm run compile` - Compiles TypeScript to JavaScript
- **Watch**: `npm run watch` - Continuous compilation during development
- **Test**: `npm run test` - Runs the test suite (requires `npm run pretest` first)
- **Pre-test**: `npm run pretest` - Compiles code and prepares test environment
- **Package**: `vsce package` - Creates `.vsix` file for distribution (requires `vsce` installed globally)

## Architecture

### Core Components

- `src/extension.ts` - Main extension entry point that:
  - Registers document and range formatting providers for Clojure language
  - Implements `runCljstyleAndFormat()` function that executes `cljstyle pipe` command
  - Handles error scenarios (executable not found, formatting failures, invalid syntax)
  - Creates output channel for logging

### Key Implementation Details

- Use
```

</details>
