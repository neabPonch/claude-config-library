---
name: gety-ai__apple-on-device-openai
source: https://github.com/gety-ai/apple-on-device-openai/blob/31a2d9b9b543bd627b3273fac936f15189a8238f/CLAUDE.md
repo: gety-ai/apple-on-device-openai
kind: claude-md
stars: 867
last_pushed: 2025-10-02T23:24:18Z
license: unknown
score: 9
domains: [macos, swiftui, backend-api, ai-integration]
tags: [swift, apple-intelligence, api-server, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# gety-ai/apple-on-device-openai — claude-md

**Why it's worth keeping:** The 'Message Flow' and 'Streaming Implementation' sections provide high-value logic patterns that prevent the AI from hallucinating standard implementations instead of following this specific one.

**Summary:** This file provides deep architectural blueprints, including data flow sequences and specific implementation details for a Swift-based API server.

**Source credibility:** High; includes highly specific technical requirements like macOS/Xcode beta versions and specialized hardware constraints.

**Recency:** Extremely current, referencing Apple Intelligence and upcoming macOS/Xcode beta specifications.

**Source:** [gety-ai/apple-on-device-openai/CLAUDE.md](https://github.com/gety-ai/apple-on-device-openai/blob/31a2d9b9b543bd627b3273fac936f15189a8238f/CLAUDE.md) · 867★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a macOS SwiftUI application that creates an OpenAI-compatible API server using Apple's on-device Foundation Models. The server exposes local Apple Intelligence models through familiar OpenAI API endpoints, enabling developers to use Apple's on-device AI with existing OpenAI-compatible tools.

**Important**: This is a GUI application (not a CLI tool) to avoid Apple's rate limiting policies for Foundation Models. Command-line tools are rate-limited, but foreground GUI apps are not.

## Requirements

- macOS 26 beta 2 or newer
- Xcode 26 beta 2 (for building)
- Apple Intelligence must be enabled in Settings > Apple Intelligence & Siri
- Device must support Apple Intelligence (Mac with Apple Silicon)

## Building and Running

### Build and run in Xcode:
```bash
open AppleOnDeviceOpenAI.xcodeproj
# Then build and run using Xcode (Cmd+R)
```

### Testing the server:
```bash
python3 test_server.py
```

The test script verifies server health, model availability, OpenAI SDK compatibility, multi-turn conversations, multilingual support, and streami
```

</details>
