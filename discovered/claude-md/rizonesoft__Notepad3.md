---
name: rizonesoft__Notepad3
source: https://github.com/rizonesoft/Notepad3/blob/afa9c739c149b22af3ea06f532048bc0e8f88ad2/CLAUDE.md
repo: rizonesoft/Notepad3
kind: claude-md
stars: 6440
last_pushed: 2026-06-11T08:00:07Z
license: unknown
score: 9
domains: [desktop-apps, systems-programming]
tags: [win32, c-cpp, architectural-mapping, side-effect-documentation]
curated: 2026-06-15
curated_by: config-scout
---

# rizonesoft/Notepad3 — claude-md

**Why it's worth keeping:** The 'touchpoint' section prevents incomplete feature implementation by detailing non-obvious dependencies like theme INIs; uses a semantic code map rather than just a file list.

**Summary:** Provides deep architectural context, specific build sequences, and critical 'easy-to-miss touchpoints' for extending the project.

**Source credibility:** Highly credible, coming from a popular/stable open-source project (6k+ stars).

**Recency:** Current; highly relevant for modern LLM-based agents performing complex refactors or feature additions.

**Source:** [rizonesoft/Notepad3/CLAUDE.md](https://github.com/rizonesoft/Notepad3/blob/afa9c739c149b22af3ea06f532048bc0e8f88ad2/CLAUDE.md) · 6440★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Guidance for Claude Code working in this repo. Read once per session; covers non-obvious mechanics and gotchas. Self-evident build/layout information is not duplicated here.

## Project

Notepad3 — Win32 C/C++ text editor on Scintilla/Lexilla. Ships with MiniPath (`Ctrl+M`) and integrates external grepWin (`Ctrl+Shift+F`) via pre-built portable exes. BSD-3. Windows-only.

## Build

Build scripts live in `Build\` (PowerShell under `Build\scripts\`):

- `Build\Build_x64.cmd [Release|Debug]` — single platform (also `_Win32`, `_ARM64`, `_x64_AVX2`)
- `Build\BuildAll.cmd` — all platforms
- `msbuild Notepad3.sln /m /p:Configuration=Release /p:Platform=x64` — CI equivalent
- `Build\Clean.cmd` — clean outputs
- Run `nuget restore Notepad3.sln` once before first build.
- Run `Version.ps1` before building to regenerate `src\VersionEx.h` (format `Major.YY.Mdd.Build`; build number in `Versions\build.txt`).
- Tests: `test\TestFileVersion.cmd`, `test\TestAhkNotepad3.cmd` (needs AutoHotkey). CI matrix in `.github/workflows/build.yml` (windows-2022).

Default configuration is Release.

## Code Map (`src\`)

| File | Purpose |
|------|---------|
| `Notepad3.c/h` | `wWinMain`, `MainWndP
```

</details>
