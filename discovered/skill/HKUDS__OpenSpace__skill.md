---
name: HKUDS__OpenSpace__skill
source: https://github.com/HKUDS/OpenSpace/blob/228f8f78073dc4ed0e63fff01c19596c50115d40/gdpval_bench/skills/ffmpeg-encoder-check-4855c0/SKILL.md
repo: HKUDS/OpenSpace
kind: skill
stars: 6532
last_pushed: 2026-06-04T13:07:06Z
license: mit
score: 7
domains: [cli-tools, media-processing]
tags: [ffmpeg, defensive-programming, environment-probing]
curated: 2026-06-15
curated_by: config-scout
---

# HKUDS/OpenSpace — skill

**Why it's worth keeping:** Demonstrates a highly transferable 'probe-verify-execute' pattern for dealing with environment-dependent CLI tools and identifies specific, high-failure libraries like libopenh264.

**Summary:** A defensive workflow instructing an agent to probe available FFmpeg encoders before attempting encoding tasks to prevent runtime failures.

**Source credibility:** High; the source repository is well-starred and actively maintained.

**Recency:** Current; the logic remains highly relevant for any agent interacting with system-level media tools.

**Source:** [HKUDS/OpenSpace/gdpval_bench/skills/ffmpeg-encoder-check-4855c0/SKILL.md](https://github.com/HKUDS/OpenSpace/blob/228f8f78073dc4ed0e63fff01c19596c50115d40/gdpval_bench/skills/ffmpeg-encoder-check-4855c0/SKILL.md) · 6532★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ffmpeg-encoder-check-4855c0
description: Check available FFmpeg encoders before writing encoding scripts to avoid library version mismatches
---

# FFmpeg Encoder Availability Check

## Purpose

Before writing any FFmpeg encoding script, always probe the system for available encoders. This prevents failures from missing or incompatible codec libraries (especially libopenh264 which frequently has version mismatches).

## Core Pattern

### Step 1: Probe Available Encoders

Always run this command before deciding on encoding parameters:

```bash
ffmpeg -encoders | grep h264
```

This shows which H.264 encoders are available on the system.

### Step 2: Choose Encoder Based on Availability

**Priority order for H.264 encoding:**

1. **`-c:v copy`** - If source and target resolution/format match, copy the stream without re-encoding (fastest, no quality loss)

2. **`-c:v libx264`** - If available, this is the most reliable and widely-compatible H.264 encoder

3. **`-c:v h264`** - Hardware acceleration if available (varies by system)

4. **Avoid `libopenh264`** - This encoder frequently has library version mismatches causing runtime failures

### Step 3: Verify Before Execution
```

</details>
