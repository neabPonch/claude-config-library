---
name: rajivm1991__DroidDock
source: https://github.com/rajivm1991/DroidDock/blob/dfd45eab81a24affcb0573bb12bd762790d768c9/CLAUDE.md
repo: rajivm1991/DroidDock
kind: claude-md
stars: 351
last_pushed: 2026-03-09T04:11:27Z
license: mit
score: 9
domains: [desktop-apps, macos, release-engineering]
tags: [release-workflow, tauri, ops]
curated: 2026-06-14
curated_by: config-scout
---

# rajivm1991/DroidDock — claude-md

**Why it's worth keeping:** The granular 'Release Checklist' is a masterclass in guiding agents through high-stakes tasks like updating Homebrew casks and GitHub Pages. It also clearly defines the project's unique use of local planning files via the `impl/` directory.

**Summary:** Provides a comprehensive operational lifecycle guide, including specific development commands and an exhaustive multi-step release process.

**Source credibility:** High; derived from a well-maintained, starred open-source macOS tool.

**Recency:** Highly current; aligns perfectly with agentic workflows requiring procedural precision.

**Source:** [rajivm1991/DroidDock/CLAUDE.md](https://github.com/rajivm1991/DroidDock/blob/dfd45eab81a24affcb0573bb12bd762790d768c9/CLAUDE.md) · 351★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

DroidDock is a macOS desktop application for browsing Android device files via ADB (Android Debug Bridge). Built with Tauri (Rust backend) + React/TypeScript frontend.

## Development Commands

```bash
npm run tauri dev          # Run development server with hot reload
npm run build              # Build TypeScript frontend
npm run tauri build        # Build production app
cd src-tauri && cargo test # Run Rust tests
```

## Git Workflow

**Branch naming:** `fix/`, `feature/`, `hotfix/`, `refactor/` prefix with descriptive name

**Standard workflow:**

1. **ALWAYS create a new branch from main when starting work on a fresh GitHub issue**: `git checkout main && git pull && git checkout -b feature/issue-description`
2. Make changes and test: `npm run build` and `cargo build`
3. Commit with issue reference: `Fixes #N`
4. Create PR: `gh pr create --title "Title" --body "Description" --reviewer rajivm1991`
5. After merge: delete branch locally and remotely, pull main

## Architecture

- **Backend:** Tauri commands in `src-tauri/src/lib.rs` with `#[tauri::comman
```

</details>
