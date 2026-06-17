---
name: chicoe__zodiac-card
source: https://github.com/chicoe/zodiac-card/blob/8452e1360a237d64dc276d6fe5a3b803eedc8285/claude.md
repo: chicoe/zodiac-card
kind: claude-md
stars: 0
last_pushed: 2026-05-01T15:37:39Z
license: other
score: 9
domains: [embedded-systems, web-frontend, hardware-interfacing]
tags: [midi, rp2040, sveltekit, firmware, protocol]
curated: 2026-06-17
curated_by: config-scout
---

# chicoe/zodiac-card — claude-md

**Why it's worth keeping:** Uses highly structured tables to define communication protocols (MIDI SysEx/CC) and detailed algorithmic breakdowns for complex state transitions like node lifecycle management. The inclusion of cross-core synchronization patterns (seqlock) is critical for hardware-focused AI coding.

**Summary:** An exceptional example of a high-density technical specification for a hardware-software hybrid project. It provides full situational awareness for both low-level firmware (RP2040) and high-level web UI (SvelteKit).

**Source credibility:** Specific, high-quality niche project with recent maintenance activity.

**Recency:** Extremely current; utilizes SvelteKit 5 and modern development standards.

**Source:** [chicoe/zodiac-card/claude.md](https://github.com/chicoe/zodiac-card/blob/8452e1360a237d64dc276d6fe5a3b803eedc8285/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Zodiac Card — Development Context

## Project Overview

Zodiac Card (formerly "Chains Sequencer") is a Markov chain sequencer for the Music Thing Modular Workshop System Computer Module. It consists of RP2040 firmware and a SvelteKit web UI that communicate via USB MIDI.

Nodes hold pitches, links set transition probabilities. Two independent chains traverse the network to generate scale-quantized melodies. The web UI displays a force-directed graph with an amber CRT visual theme.

## Architecture

### Dual-Core RP2040

- **Core 0**: `ProcessSample()` at 24kHz — audio synthesis, clock processing, chain traversal, LED output, pending edit consumption
- **Core 1**: `MIDICore()` — USB MIDI CC/SysEx communication with browser UI, reads graph state via seqlock

Cross-core synchronization uses a **seqlock pattern** (`graphSeq`): Core 0 increments before and after writes (odd = writing), Core 1 retries reads if the sequence number changed or is odd.

### Web UI (SvelteKit 5)

- **Static adapter** — builds to `web/build/` for hosting or embedding
- **d3-force** for force-directed graph layout
- **WebMIDI API** for real-time communication (Chrome/Chromium only, requires SysEx permission)
```

</details>
