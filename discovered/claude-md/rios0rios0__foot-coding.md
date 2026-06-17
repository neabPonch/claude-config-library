---
name: rios0rios0__foot-coding
source: https://github.com/rios0rios0/foot-coding/blob/9fbad89f2b0bc90896f1a405f71280b61356cec6/CLAUDE.md
repo: rios0rios0/foot-coding
kind: claude-md
stars: 2
last_pushed: 2026-05-25T19:50:19Z
license: gpl-3.0
score: 8
domains: [legacy-systems, desktop-apps, low-level]
tags: [legacy-code, negative-constraints, win32, assembly]
curated: 2026-06-15
curated_by: config-scout
---

# rios0rios0/foot-coding — claude-md

**Why it's worth keeping:** Uses 'negative constraints' (what NOT to do) which is vital for legacy code, and provides explicit warnings about assembly implementations that an LLM would otherwise attempt to 'fix'.

**Summary:** Establishes strict behavioral boundaries for a legacy project to prevent unwanted modernization or refactoring. It defines exact constraints on architecture, language, and low-level implementation details.

**Source credibility:** Niche personal project with minimal stars but highly specialized documentation.

**Recency:** Highly relevant; addresses the tendency of modern LLMs to suggest refactors or framework migrations.

**Source:** [rios0rios0/foot-coding/CLAUDE.md](https://github.com/rios0rios0/foot-coding/blob/9fbad89f2b0bc90896f1a405f71280b61356cec6/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Foot Coding is a **discontinued** Windows desktop application (Object Pascal / Borland Delphi 7). Discontinued 2013-11-23. No new features or bug fixes are planned. The repository is preserved as a historical and educational reference.

## Architecture

Single-file Win32 API application — no VCL framework. `FC.dpr` contains all window creation, message handling, and UI. `External Uses/MyUtils.pas` contains all conversion algorithms. GUI controls are created manually via `CreateWindowExA` and dispatched through a single `WindowProc` callback.

`IntToStr` and `StrToInt` in `MyUtils.pas` are implemented in pure x86 assembly. Do not replace them with Pascal equivalents.

## Build

No automated build system, CI, or tests. Open `FC.dpr` in Borland Delphi 7, press F9. Run `Clear.bat` to remove build artifacts before committing.

## Conventions

- **Discontinued** — do not suggest feature additions, library upgrades, or framework migration (VCL/FMX).
- **No VCL** — do not introduce VCL or third-party component packages.
- **No external dependencies** — `MyUtils.
```

</details>
