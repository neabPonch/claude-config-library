---
name: babysor__MockingBird__skill
source: https://github.com/babysor/MockingBird/blob/28dc5e14f12d7c754612af2fde8e78a4b03f8616/skills/speak/SKILL.md
repo: babysor/MockingBird
kind: skill
stars: 36899
last_pushed: 2026-03-03T14:59:58Z
license: other
score: 8
domains: [audio-generation, cli-tools, multimedia]
tags: [tts, voice-cloning, dubbing]
curated: 2026-06-15
curated_by: config-scout
---

# babysor/MockingBird — skill

**Why it's worth keeping:** The 'Timeline Mode' provides a structured way for an agent to perform granular, cinematic audio orchestration via JSON control files. This allows the agent to act as a director rather than just a speaker.

**Summary:** A sophisticated toolset for text-to-speech, voice cloning, and time-aligned audio rendering. It enables complex dubbing workflows through SRT and JSON-based voice mapping.

**Source credibility:** Extremely high; the repo has 36k+ stars and recent maintenance activity.

**Recency:** Current; highly compatible with modern agentic CLI-driven workflows.

**Source:** [babysor/MockingBird/skills/speak/SKILL.md](https://github.com/babysor/MockingBird/blob/28dc5e14f12d7c754612af2fde8e78a4b03f8616/skills/speak/SKILL.md) · 36899★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: speak
description: Convert text into speech with Kokoro or Noiz, including simple and timeline-aligned modes.
---

# speak

Convert any text into speech audio. Supports two backends (Kokoro local, Noiz cloud), two modes (simple or timeline-accurate), and per-segment voice control.

## Triggers

- text to speech / speak / say / tts
- voice clone / dubbing 
- epub to audio / srt to audio / convert to audio

## Simple Mode — text to audio

```bash
# Kokoro (auto-detected when installed)
bash skills/speak/scripts/tts.sh speak -t "Hello world" -v af_sarah -o hello.wav
bash skills/speak/scripts/tts.sh speak -f article.txt -v zf_xiaoni --lang cmn -o out.mp3 --format mp3

# Noiz (auto-detected when NOIZ_API_KEY is set, or force with --backend noiz)
# If --voice-id is omitted, the script prints 5 available built-in voices and exits.
# Pick one from the output and re-run with --voice-id <id>.
bash skills/speak/scripts/tts.sh speak -f input.txt --voice-id voice_abc --auto-emotion --emo '{"Joy":0.5}' -o out.wav

# Noiz: optional --duration (float, seconds, range (0, 36]) for target audio length
bash skills/speak/scripts/tts.sh speak -t "Short line" --voice-id voice_abc --duration 3.5
```

</details>
