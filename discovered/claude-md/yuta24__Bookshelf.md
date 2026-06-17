---
name: yuta24__Bookshelf
source: https://github.com/yuta24/Bookshelf/blob/c96f6cf633c47093a2d80a704cc4cfd44ee00959/CLAUDE.md
repo: yuta24/Bookshelf
kind: claude-md
stars: 1
last_pushed: 2026-06-12T00:01:49Z
license: mit
score: 7
domains: [ios-development, swift]
tags: [tca, swiftui, modular-architecture]
curated: 2026-06-16
curated_by: config-scout
---

# yuta24/Bookshelf — claude-md

**Why it's worth keeping:** It effectively defines the responsibility of different modules and explicitly points out where generated code lives to prevent LLM confusion.

**Summary:** This config maps out a modular iOS architecture using The Composable Architecture (TCA) and provides essential development commands via Makefiles.

**Source credibility:** Single-star repository, but appears to be a structured, active personal project.

**Recency:** Very current; uses modern Swift standards like NavigationStack and async/await.

**Source:** [yuta24/Bookshelf/CLAUDE.md](https://github.com/yuta24/Bookshelf/blob/c96f6cf633c47093a2d80a704cc4cfd44ee00959/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Swift iOS bookshelf application built with SwiftUI and The Composable Architecture (TCA). The app allows users to manage their book collection with features like scanning, tagging, and statistics.

## Architecture

The project follows a modular architecture with four main Swift packages:

### Core Package (`Core/`)
- **Models**: BookModel, GenreModel, RemindModel, SyncModel - Domain entities
- **Clients**: Abstract interfaces for external services (BookClient, SearchClient, etc.)
- **Features**: TCA reducers and business logic (BookCore, SettingsCore, StatisticsCore)
- Uses The Composable Architecture as the primary state management framework

### Infrastructure Package (`Infrastructure/`)  
- **Live Implementations**: Concrete implementations of Core clients (BookClientLive, SearchClientLive, etc.)
- **Data Layer**: Core Data models (BookRecord, TagRecord) and persistence logic
- **External Services**: Firebase integration for analytics, remote config, and push notifications

### Presentation Package (`Presentation/`)
- **SwiftUI Views
```

</details>
