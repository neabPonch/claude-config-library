---
name: illixion__vscode-vibrancy-continued__claude
source: https://github.com/illixion/vscode-vibrancy-continued/blob/cbab8fe717da2bbb6678914f98f36237bc52d5a6/.claude/CLAUDE.md
repo: illixion/vscode-vibrancy-continued
kind: claude-md
stars: 837
last_pushed: 2026-06-10T20:40:07Z
license: mit
score: 9
domains: [vscode-extension, desktop-app]
tags: [system-level, platform-specific, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# illixion/vscode-vibrancy-continued — claude-md

**Why it's worth keeping:** It documents non-obvious edge cases (like the VSCode 1.95 file merge quirk and Windows file locking) that prevent an AI from introducing breaking changes during refactoring.

**Summary:** Maps out system architecture and critical platform-specific file manipulation patterns for a tool that modifies VS Code's internal files.

**Source credibility:** High; a popular, highly-starred project with very active maintenance.

**Recency:** Current; specifically addresses recent VS Code versioning changes (1.95+).

**Source:** [illixion/vscode-vibrancy-continued/.claude/CLAUDE.md](https://github.com/illixion/vscode-vibrancy-continued/blob/cbab8fe717da2bbb6678914f98f36237bc52d5a6/.claude/CLAUDE.md) · 837★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Project Overview

VSCode extension that applies vibrancy/transparency effects to the Visual Studio Code UI. Works by modifying VSCode's internal files (workbench HTML, main JS, Electron JS) and injecting runtime modules.

## Key Architecture

### Extension entry point
- `extension/index.js` — Main extension logic: install, uninstall, update flows
- `extension/elevated-file-writer.js` — Cross-platform elevated file operations (UAC on Windows, pkexec on Linux, osascript on macOS)
- `extension/platform.js` — Platform detection
- `extension/uninstallHook.js` — Cleanup on extension uninstall

### Runtime modules
- `runtime/` — ESM runtime injected into VSCode's workbench (modern VSCode)
- `runtime-pre-esm/` — CJS runtime for older VSCode versions
- `native/` — C++ native modules for Windows vibrancy effects; prebuilt binaries in `native/prebuilt/`

### Themes and i18n
- `themes/` — Theme configuration and CSS files
- `package.nls.json`, `package.nls.ja.json`, `package.nls.zh-CN.json` — Localization strings

## Important Patterns

### StagedFileWriter (elevated-file-writer.js)
All file modifications to VSCode's install directory go through `StagedFileWriter`. When elevation is needed,
```

</details>
