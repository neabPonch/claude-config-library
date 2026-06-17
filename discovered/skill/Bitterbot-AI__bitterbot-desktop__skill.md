---
name: Bitterbot-AI__bitterbot-desktop__skill
source: https://github.com/Bitterbot-AI/bitterbot-desktop/blob/9a53cc29f984b12d2c280b008fbdc17c7997b362/skills/songsee/SKILL.md
repo: Bitterbot-AI/bitterbot-desktop
kind: skill
stars: 2382
last_pushed: 2026-06-14T18:14:19Z
license: other
score: 8
domains: [cli-tools, audio-processing, data-visualization]
tags: [spectrograms, command-line, media]
curated: 2026-06-15
curated_by: config-scout
---

# Bitterbot-AI/bitterbot-desktop — skill

**Why it's worth keeping:** It provides a perfect template of high-density command examples (Quick start) followed by exhaustive flag definitions, minimizing agent hallucination during tool use.

**Summary:** A specialized skill file for the songsee CLI that enables an agent to generate audio spectrograms and feature visualizations.

**Source credibility:** High; the source repository is popular with significant stars and active maintenance.

**Recency:** Current; utilizes structured metadata suitable for modern agentic workflows.

**Source:** [Bitterbot-AI/bitterbot-desktop/skills/songsee/SKILL.md](https://github.com/Bitterbot-AI/bitterbot-desktop/blob/9a53cc29f984b12d2c280b008fbdc17c7997b362/skills/songsee/SKILL.md) · 2382★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: songsee
description: Generate spectrograms and feature-panel visualizations from audio with the songsee CLI.
homepage: https://github.com/steipete/songsee
metadata:
  {
    "bitterbot":
      {
        "emoji": "🌊",
        "requires": { "bins": ["songsee"] },
        "install":
          [
            {
              "id": "brew",
              "kind": "brew",
              "formula": "steipete/tap/songsee",
              "bins": ["songsee"],
              "label": "Install songsee (brew)",
            },
          ],
      },
  }
---

# songsee

Generate spectrograms + feature panels from audio.

Quick start

- Spectrogram: `songsee track.mp3`
- Multi-panel: `songsee track.mp3 --viz spectrogram,mel,chroma,hpss,selfsim,loudness,tempogram,mfcc,flux`
- Time slice: `songsee track.mp3 --start 12.5 --duration 8 -o slice.jpg`
- Stdin: `cat track.mp3 | songsee - --format png -o out.png`

Common flags

- `--viz` list (repeatable or comma-separated)
- `--style` palette (classic, magma, inferno, viridis, gray)
- `--width` / `--height` output size
- `--window` / `--hop` FFT settings
- `--min-freq` / `--max-freq` frequency range
- `--start` / `--duration` time slice
- `--format` jpg
```

</details>
