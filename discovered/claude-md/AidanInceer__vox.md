---
name: AidanInceer__vox
source: https://github.com/AidanInceer/vox/blob/abda51f7db3c8f7a463ec46ac7995b21662484a9/claude.md
repo: AidanInceer/vox
kind: claude-md
stars: 0
last_pushed: 2026-01-25T12:46:24Z
license: mit
score: 9
domains: [cli-tools, audio-processing]
tags: [architecture-focus, ascii-diagrams, workflow-mapping]
curated: 2026-06-14
curated_by: config-scout
---

# AidanInceer/vox — claude-md

**Why it's worth keeping:** The use of data flow diagrams shows exactly how information traverses the system, which is invaluable for preventing logic errors during refactoring. It provides a structural mental model that simple file trees cannot match.

**Summary:** Provides high-density architectural context using ASCII system diagrams and module responsibility mappings.

**Source credibility:** Low social proof (0 stars), but the documentation indicates high-quality, human-curated technical writing.

**Recency:** 5 months old; highly relevant to current Claude Code and agentic workflows.

**Source:** [AidanInceer/vox/claude.md](https://github.com/AidanInceer/vox/blob/abda51f7db3c8f7a463ec46ac7995b21662484a9/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Development Guidelines for vox

## Project Overview

**vox** is a bidirectional audio-text conversion CLI tool for Windows 11 that enables:
- **Text-to-Speech (TTS)**: Read web content aloud from URLs, browser tabs, or HTML files using offline neural TTS
- **Speech-to-Text (STT)**: Transcribe voice recordings to text using Whisper-powered offline recognition

**Target Users**: Windows 11 users who need accessibility features, hands-free content consumption, or voice transcription capabilities without cloud dependencies.

**Key Design Philosophy**:
- **Offline-first**: No API keys, no cloud services, complete privacy
- **Test-driven**: ≥80% coverage requirement, ≥95% for critical paths
- **Simple UX**: CLI-based with intuitive commands and keyboard controls
- **Modular architecture**: Clear separation between TTS, STT, extraction, and session management

**Version**: 3.0.0 (MAJOR bump for rebranding from "vox" to "vox" with breaking CLI changes)

---

## Architecture Overview

### System Architecture

```
┌───────────────────────────────────────────────────────────┐
│                        vox CLI                            │
│                     (src/main.py)
```

</details>
