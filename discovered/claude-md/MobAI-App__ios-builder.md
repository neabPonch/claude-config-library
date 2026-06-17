---
name: MobAI-App__ios-builder
source: https://github.com/MobAI-App/ios-builder/blob/bf9f82b3ffbd9c58e4ecf92553438aea36c2ede0/CLAUDE.md
repo: MobAI-App/ios-builder
kind: claude-md
stars: 472
last_pushed: 2026-03-31T15:33:32Z
license: mit
score: 9
domains: [cli-tools, ios-development, go]
tags: [go, ios, github-actions, devops]
curated: 2026-06-15
curated_by: config-scout
---

# MobAI-App/ios-builder — claude-md

**Why it's worth keeping:** The use of ASCII flowcharts to map complex logic paths is excellent for LLM understanding, and the 'Key Patterns' section provides high-level technical context rather than just file locations.

**Summary:** A comprehensive guide for a Go-based iOS development CLI tool that includes build commands, architectural flows, and platform-specific requirements.

**Source credibility:** High; a well-starred (472) project with recent maintenance activity.

**Recency:** Very current; uses modern Go patterns and contemporary iOS/Flutter workflows.

**Source:** [MobAI-App/ios-builder/CLAUDE.md](https://github.com/MobAI-App/ios-builder/blob/bf9f82b3ffbd9c58e4ecf92553438aea36c2ede0/CLAUDE.md) · 472★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Builder** is a Go CLI tool for iOS development without a Mac. It has two main capabilities:
1. **Remote builds**: Build iOS apps via GitHub Actions from any platform
2. **Dev tools**: Hot reload on real iOS devices using MobAI (Flutter and React Native)

## Build Commands

```bash
# Build
go build -o builder ./cmd/builder

# Test
go test ./...

# Install
go install ./cmd/builder

# Run
./builder auth github       # Authenticate with GitHub (OAuth device flow)
./builder init              # Set up workflow in current repo
./builder ios build         # Trigger build and download IPA to ./dist/
./builder dev flutter       # Flutter hot reload with MobAI
./builder dev rn            # React Native hot reload with MobAI
./builder dev flutter --skip-install --bundle-id <id>  # Use already installed app
./builder dev rn --skip-install --bundle-id <id>       # Use already installed app
```

## Architecture

```
builder auth github ─────► GitHub OAuth (device flow)
                                │
                                ▼
```

</details>
