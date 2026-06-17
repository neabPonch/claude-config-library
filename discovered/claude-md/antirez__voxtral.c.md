---
name: antirez__voxtral.c
source: https://github.com/antirez/voxtral.c/blob/134d366c24d20c64b614a3dcc8bda2a6922d077d/CLAUDE.md
repo: antirez/voxtral.c
kind: claude-md
stars: 1692
last_pushed: 2026-02-15T18:58:52Z
license: mit
score: 9
domains: [cli-tools, ml-inference, audio-processing, c-programming]
tags: [C, Inference, Streaming]
curated: 2026-06-15
curated_by: config-scout
---

# antirez/voxtral.c — claude-md

**Why it's worth keeping:** The 'Development Rules' section sets strict constraints on complexity and portability, while the 'Streaming Architecture' explanation provides necessary mental models for modifying core logic.

**Summary:** Provides essential architectural context for streaming audio-to-text inference alongside precise command-line usage patterns.

**Source credibility:** High; authored by antirez (creator of Redis) with significant star count and recent updates.

**Recency:** Very current, including modern hardware acceleration targets like Apple Silicon/Metal.

**Source:** [antirez/voxtral.c/CLAUDE.md](https://github.com/antirez/voxtral.c/blob/134d366c24d20c64b614a3dcc8bda2a6922d077d/CLAUDE.md) · 1692★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Voxtral Realtime 4B - Project Instructions

Pure C implementation of Mistral AI's Voxtral Realtime 4B speech-to-text model.
HuggingFace: `mistralai/Voxtral-Mini-4B-Realtime-2602`

![demo](samples/demo.gif)

## Quick Reference

```bash
# Build
make mps       # Apple Silicon (fastest)
make blas      # CPU with BLAS (Accelerate on macOS, OpenBLAS on Linux)
make clean

# Test (slow — needs fast Apple Silicon GPU, ~2 min on M3/M4 Max)
make test

# Run (tokens stream to stdout as generated)
./voxtral -d voxtral-model -i audio.wav            # default: timing info on stderr
./voxtral -d voxtral-model -i audio.wav --silent    # no stderr output
./voxtral -d voxtral-model -i audio.wav --debug     # per-layer/per-chunk details
./voxtral -d voxtral-model -i audio.wav --alt 0.5   # show alternative tokens inline

# Microphone input (macOS only, Ctrl+C to stop)
./voxtral -d voxtral-model --from-mic               # default: 2s processing interval
./voxtral -d voxtral-model --from-mic -I 1.0         # 1s interval for lower latency

# Stdin input (auto-detects WAV vs raw s16le 16kHz mono)
cat audio.wav | ./voxtral -d voxtral-model --stdin
ffmpeg -i samples/I_have_a_dream.ogg -f s16le -ar 16000 -
```

</details>
