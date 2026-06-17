---
name: sudip-mondal-2002__Amplitron
source: https://github.com/sudip-mondal-2002/Amplitron/blob/7a09319192e21cca5993ac6d0dadfc49146e1021/CLAUDE.md
repo: sudip-mondal-2002/Amplitron
kind: claude-md
stars: 58
last_pushed: 2026-06-14T09:56:29Z
license: mit
score: 9
domains: [dsp, audio-engineering, c++, real-time]
tags: [architecture, concurrency, dsp, low-latency]
curated: 2026-06-15
curated_by: config-scout
---

# sudip-mondal-2002/Amplitron — claude-md

**Why it's worth keeping:** It provides critical constraints on concurrency (lock-free/try_lock protocols) and threading priorities, which is essential for an AI to avoid introducing latency or race conditions in real-time systems.

**Summary:** A high-level architectural blueprint defining 'Agents' as encapsulated, thread-aware entities within a real-time DSP environment. It maps out responsibilities across audio, GUI, and MIDI threads.

**Source credibility:** A well-structured personal project with active development and significant community interest (58 stars).

**Recency:** Current; reflects modern high-performance C++ development standards.

**Source:** [sudip-mondal-2002/Amplitron/CLAUDE.md](https://github.com/sudip-mondal-2002/Amplitron/blob/7a09319192e21cca5993ac6d0dadfc49146e1021/CLAUDE.md) · 58★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Amplitron Processing Agents & System Architecture

This document outlines the **Agent Architecture** and C++ coding paradigm within the Amplitron Guitar Amp Simulator. In this high-performance real-time DSP (Digital Signal Processing) environment, an "Agent" is an autonomous, encapsulated component responsible for specific processing, coordination, or state management tasks.

These agents operate concurrently across high-priority audio threads, MIDI callback threads, and UI threads to achieve ultra-low latency (~1.3ms) and glitch-free, real-time performance.

---

## 1. System-Level Coordination Agents

These core manager agents oversee the lifecycle, thread boundaries, and hardware interactions of the Amplitron ecosystem.

### 1.1 The Audio Engine Agent (`src/audio/engine/audio_engine.cpp`)
The master coordinator of the system, running at the highest OS priority via a platform driver backend.
* **Role:** Manages the real-time audio callback loop, fetching inputs from raw mono float32 hardware and routing them through the dynamic signal chain.
* **Responsibilities:**
  * Auto-detecting input/output hardware and highlighted USB guitar cables.
  * Negotiating buffer sizes (32 to 51
```

</details>
