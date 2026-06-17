---
name: snowplow__snowplow-unity-tracker
source: https://github.com/snowplow/snowplow-unity-tracker/blob/88f1c541953bfaf628f9b2e90449acb23782c624/CLAUDE.md
repo: snowplow/snowplow-unity-tracker
kind: claude-md
stars: 17
last_pushed: 2026-05-19T12:54:01Z
license: apache-2.0
score: 9
domains: [csharp, unity-engine]
tags: [architectural-patterns, platform-specific, correct-vs-wrong]
curated: 2026-06-14
curated_by: config-scout
---

# snowplow/snowplow-unity-tracker — claude-md

**Why it's worth keeping:** Uses 'Correct vs Wrong' code blocks to define design patterns (Builder/Async) and includes mission-critical environment setup/test instructions.

**Summary:** A highly structured technical guide that establishes architectural constraints, platform-specific logic, and coding standards for a C# Unity library.

**Source credibility:** High-quality documentation for a specialized analytics tool; content is purpose-built for AI assistance.

**Recency:** Highly relevant and current with modern LLM interaction techniques.

**Source:** [snowplow/snowplow-unity-tracker/CLAUDE.md](https://github.com/snowplow/snowplow-unity-tracker/blob/88f1c541953bfaf628f9b2e90449acb23782c624/CLAUDE.md) · 17★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Snowplow Unity Tracker - Claude Code Documentation

## Project Overview
The Snowplow Unity Tracker is a C# library for Unity that enables event tracking and analytics in Unity games and applications. It sends events to Snowplow collectors for data analysis, supporting multiple platforms including iOS, Android, Windows, Mac, Linux, and WebGL.

## Development Commands
```bash
# Build the tracker library
cd SnowplowTracker && dotnet build

# Run tests (requires Unity 2021.3.12f1 LTS)
# Open SnowplowTracker.Tests in Unity Editor
# Window -> General -> Test Runner -> EditMode -> Run All

# Start test collector (requires Vagrant)
vagrant up && vagrant ssh
cd /vagrant && mb &
curl -X POST -d @/vagrant/Resources/imposter.json http://localhost:2525/imposters

# Build demo game
# Open SnowplowTracker.Demo in Unity Editor and build
```

## Architecture
The tracker follows a layered architecture with clear separation of concerns:

### Core Components
- **Tracker**: Main entry point for event tracking operations
- **Emitter**: Handles event transmission (AsyncEmitter, SyncEmitter, WebGlEmitter)
- **Storage**: Event persistence using LiteDB or in-memory storage
- **Events**: Strongly-typed eve
```

</details>
