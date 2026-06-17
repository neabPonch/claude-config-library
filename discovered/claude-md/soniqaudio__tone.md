---
name: soniqaudio__tone
source: https://github.com/soniqaudio/tone/blob/de055fe77eb4ce49c5775833d80bb2e7c3e02c21/claude.md
repo: soniqaudio/tone
kind: claude-md
stars: 8
last_pushed: 2025-11-16T21:30:47Z
license: unknown
score: 9
domains: [web-frontend, audio-engineering, creative-tools]
tags: [zustand, nextjs, canvas, audio-engine, technical-debt]
curated: 2026-06-16
curated_by: config-scout
---

# soniqaudio/tone — claude-md

**Why it's worth keeping:** The 'Known Issues & Technical Debt' section is exceptional for guiding AI away from existing bugs; it also details low-level implementation logic like the audio scheduler and layer-based canvas approach.

**Summary:** Provides deep architectural context for a complex audio engine, including specific state management patterns and canvas rendering strategies.

**Source credibility:** A niche open-source music production project with clear architectural documentation.

**Recency:** Current as of mid-2024, providing relevant context for modern web tech stacks.

**Source:** [soniqaudio/tone/claude.md](https://github.com/soniqaudio/tone/blob/de055fe77eb4ce49c5775833d80bb2e7c3e02c21/claude.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude.md - Tone DAW Project Context

## Project Overview

**Tone** (also referred to as "tonedaw") is an open-source web-based Digital Audio Workstation (DAW) inspired by FL Studio, Ableton Live, and similar professional music production software. The project is being developed for the **soniqaudio** brand.

### Key Characteristics
- **Next.js 16** with TypeScript
- **React 19** for UI
- **Zustand** for state management
- **Tone.js** and **soundfont-player** for audio playback
- **TypeScript** 
- **Biome for Linting/Formatting** 
- **Canvas-based** piano roll editor (ported from earlier work)
- Focus on MIDI recording, editing, and audio playback

### Current State
The project is in a **good foundational state** with:
- Functional piano roll editor with note editing, velocity editing, ghost notes
- MIDI recording and playback
- Transport controls (play, pause, stop, loop)
- Metronome
- Basic track system
- View switching (Piano Roll, Playlist, Mixer - latter two are mockups)

**Important Note**: Every line of code has been AI-written, so nothing should be assumed perfect. Always verify and review.

---

## Architecture Decisions

### Pattern System
- **FL Studio-style pattern-ba
```

</details>
