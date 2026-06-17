---
name: cwtools__cwtools-vscode
source: https://github.com/cwtools/cwtools-vscode/blob/364beae5e3c1edfd6fe2f7e5701e8df93c9e45c5/CLAUDE.md
repo: cwtools/cwtools-vscode
kind: claude-md
stars: 111
last_pushed: 2026-02-14T10:07:19Z
license: other
score: 8
domains: [vscode-extensions, dot-net, typescript]
tags: [hybrid-build, language-server, vs-code]
curated: 2026-06-15
curated_by: config-scout
---

# cwtools/cwtools-vscode — claude-md

**Why it's worth keeping:** Clearly differentiates between multi-language build steps (F# vs TypeScript) and provides OS-specific commands which prevents tool errors during compilation.

**Summary:** Provides a structured guide for a hybrid .NET/TypeScript VS Code extension, covering both backend and frontend build pipelines.

**Source credibility:** The project has respectable star count and recent maintenance activity.

**Recency:** Very recent, consistent with modern development workflows.

**Source:** [cwtools/cwtools-vscode/CLAUDE.md](https://github.com/cwtools/cwtools-vscode/blob/364beae5e3c1edfd6fe2f7e5701e8df93c9e45c5/CLAUDE.md) · 111★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

CWTools is a Visual Studio Code extension that provides language services for Paradox Interactive game modding, supporting games like Stellaris, Hearts of Iron IV, Europa Universalis IV, Crusader Kings II/III, Victoria 2/3, and Imperator: Rome. The extension offers syntax validation, autocomplete, tooltips, localization checking, and visual graph analysis for game scripts.

## Architecture

This is a hybrid .NET/TypeScript VS Code extension with three main components:

### Backend (.NET/F#)
- **Main** (`src/Main/`): Core F# language server providing validation, completion, and analysis
- **LSP** (`src/LSP/`): Language Server Protocol implementation in F#  
- **CSharpExtensions** (`src/CSharpExtensions/`): C# helper utilities
- Dependencies: Uses CWTools library via Paket (git submodule in `paket-files/`)

### Frontend (TypeScript)
- **Client Extension** (`client/extension/`): VS Code extension host and commands
- **Webview** (`client/webview/`): Graph visualization using Cytoscape.js
- **Test Suite** (`client/test/`): Extension tests with sample
```

</details>
