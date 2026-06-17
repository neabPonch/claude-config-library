---
name: bretbouchard__white-room-pedalboard__claude
source: https://github.com/bretbouchard/white-room-pedalboard/blob/b2a0804a619df6779c169c516af9fa580e55c8b3/.claude/CLAUDE.md
repo: bretbouchard/white-room-pedalboard
kind: claude-md
stars: 0
last_pushed: 2026-01-22T17:36:32Z
license: unknown
score: 9
domains: [audio-engineering, systems-architecture, ai-agents]
tags: [architecture-contract, hierarchical-memory, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# bretbouchard/white-room-pedalboard — claude-md

**Why it's worth keeping:** It provides rigid structural constraints to prevent architectural debt and demonstrates how to instruct an agent to manage its own long-term context via specialized tools.

**Summary:** Defines a strict architectural contract for multi-repo plugin development and implements 'Confucius,' a hierarchical memory system for pattern retention.

**Source credibility:** High technical depth in audio engineering (JUCE/DSP) despite low public visibility.

**Recency:** Current; highly relevant to modern agentic tool-use patterns.

**Source:** [bretbouchard/white-room-pedalboard/.claude/CLAUDE.md](https://github.com/bretbouchard/white-room-pedalboard/blob/b2a0804a619df6779c169c516af9fa580e55c8b3/.claude/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# White Room Project - Claude AI Instructions

## Project Overview

White Room is a next-generation audio plugin development environment integrating JUCE backend (C++), Swift frontend, and Python tooling with AI-driven development workflows.

## Core Development Principles

### 🎸 **PLUGIN ARCHITECTURE CONTRACT (MANDATORY)**

**⚠️ CRITICAL: EVERY instrument/effect MUST follow these rules:**

1. **Separate Repository**: Each instrument/effect has its own GitHub repo
   - Example: `https://github.com/bretbouchard/biPhase.git`
   - NEVER add to `audio_agent_juce` repo directly

2. **Standard Folder Structure**:
   ```
   [NAME]/
   ├── plugins/              ← REQUIRED ROOT FOLDER
   │   ├── dsp/              ← Pure DSP (no wrapper)
   │   ├── vst/              ← VST3 build output
   │   ├── au/               ← AU build output
   │   ├── clap/             ← CLAP build output
   │   ├── lv2/              ← LV2 build output
   │   ├── auv3/             ← iOS AUv3 build output
   │   └── standalone/       ← Standalone app
   ├── include/              ← DSP headers
   ├── src/                  ← DSP implementation
   ├── tests/                ← Test harness
   ├── presets/              ← Fa
```

</details>
