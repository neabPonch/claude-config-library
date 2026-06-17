---
name: peixotorms__tabby-claude-fix
source: https://github.com/peixotorms/tabby-claude-fix/blob/e20170900226d7aef45b0ca5517a56c59000e788/CLAUDE.md
repo: peixotorms/tabby-claude-fix
kind: claude-md
stars: 0
last_pushed: 2026-03-25T19:41:35Z
license: unknown
score: 7
domains: [cli-tools, web-frontend]
tags: [component-mapping, typescript]
curated: 2026-06-17
curated_by: config-scout
---

# peixotorms/tabby-claude-fix — claude-md

**Why it's worth keeping:** The explicit inclusion of file paths and line ranges for key components reduces 'searching' time for the agent. It also documents complex logic edge cases like SplitTabComponent traversal.

**Summary:** Describes a specialized terminal plugin, providing specific mappings between architectural components and their code locations.

**Source credibility:** Low social proof with 0 stars, suggesting a niche personal utility project.

**Recency:** Current; reflects modern TypeScript/Angular development patterns.

**Source:** [peixotorms/tabby-claude-fix/CLAUDE.md](https://github.com/peixotorms/tabby-claude-fix/blob/e20170900226d7aef45b0ca5517a56c59000e788/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

**KEEP IT SIMPLE**
This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Tabby terminal plugin that adds Shift+Enter hotkey functionality to send a backslash newline (`\\\n`) in terminal sessions. The plugin is built using Angular and TypeScript, following Tabby's plugin architecture.

## Build Commands

```bash
# Compile TypeScript to JavaScript
npx tsc

# Watch mode for development
npx tsc --watch
```

## Architecture

### Key Components

1. **ShiftEnterHotkeyProvider** (src/index.ts:11-20): Registers the `shift-enter-newline` hotkey with Tabby's hotkey system
2. **ShiftEnterHandler** (src/index.ts:23-135): Core logic that handles the Shift+Enter event and sends `\\\n` to active terminal
3. **ShiftEnterModule** (src/index.ts:147-151): Angular module that registers providers and initializes the handler

### Integration with Tabby

The plugin integrates with Tabby through:
- `HotkeyProvider`: Multi-provider pattern to register custom hotkeys
- `HotkeysService`: Subscribe to hotkey events
- `AppService`: Access active tabs and terminal sessions
- Terminal session access via `tab.session`, `
```

</details>
