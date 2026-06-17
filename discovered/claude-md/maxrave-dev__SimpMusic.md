---
name: maxrave-dev__SimpMusic
source: https://github.com/maxrave-dev/SimpMusic/blob/c4c4ddb246f3a6e25354636ddf7e0af903d2f570/CLAUDE.md
repo: maxrave-dev/SimpMusic
kind: claude-md
stars: 9510
last_pushed: 2026-06-07T14:45:00Z
license: gpl-3.0
score: 9
domains: [mobile-app, android, kotlin]
tags: [clean-architecture, research-workflow, multi-module]
curated: 2026-06-15
curated_by: config-scout
---

# maxrave-dev/SimpMusic — claude-md

**Why it's worth keeping:** The 'Research Before Implementation' section is an elite instruction set that forces the AI to validate libraries and patterns via documentation/web search; the module dependency diagram prevents architectural drift.

**Summary:** A highly structured guide for a complex multi-module Kotlin project that includes a rigorous mandatory research workflow.

**Source credibility:** High; comes from a popular open-source project (9.5k stars) with recent activity.

**Recency:** Very current; explicitly utilizes MCP tool-use workflows for research.

**Source:** [maxrave-dev/SimpMusic/CLAUDE.md](https://github.com/maxrave-dev/SimpMusic/blob/c4c4ddb246f3a6e25354636ddf7e0af903d2f570/CLAUDE.md) · 9510★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - SimpMusic Project Guide for AI Agents

## 🌐 Language Rule

**Response language**: Always respond in **English**, and after each sentence, add a **Vietnamese translation in parentheses**.
Example: "Hello, how are you? (Xin chào, bạn khỏe không?)"

This applies to all conversations in this project. The user is using Max plan so token cost is not a concern.

## 📋 Project Overview

**SimpMusic** is a FOSS (Free and Open Source Software) YouTube Music client for Android and Desktop, built with Compose Multiplatform.

### Main Purpose
- Stream music from YouTube Music and YouTube for free, ad-free, with background playback
- Provide advanced features like Spotify Canvas, AI song suggestions, synced lyrics
- Support both Android and Desktop (Windows, macOS, Linux)

### Basic Information
- **Package name**: `com.maxrave.simpmusic`
- **Primary language**: Kotlin
- **UI Framework**: Jetpack Compose / Compose Multiplatform
- **Architecture**: Clean Architecture + MVVM
- **Build system**: Gradle (Kotlin DSL)

## 🏗️ Architecture

### Clean Architecture Layers

```
┌─────────────────────────────────────┐
│  Presentation Layer (UI)            │
│  - Jetpack Compose / Compose MP
```

</details>
