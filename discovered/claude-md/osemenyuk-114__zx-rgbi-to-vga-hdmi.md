---
name: osemenyuk-114__zx-rgbi-to-vga-hdmi
source: https://github.com/osemenyuk-114/zx-rgbi-to-vga-hdmi/blob/18b79607b0bc713d0d1d85c8841bf6395b9e843d/CLAUDE.md
repo: osemenyuk-114/zx-rgbi-to-vga-hdmi
kind: claude-md
stars: 20
last_pushed: 2026-06-14T19:01:02Z
license: gpl-3.0
score: 9
domains: [embedded-systems, firmware, c]
tags: [rp2040, platformio, pio, hardware-interfacing]
curated: 2026-06-15
curated_by: config-scout
---

# osemenyuk-114/zx-rgbi-to-vga-hdmi — claude-md

**Why it's worth keeping:** Uses high-value sections like 'Key Concepts' feature flag tables and 'Development Notes' that explicitly warn against specific architectural anti-patterns.

**Summary:** Provides deep technical context for complex embedded firmware including file-to-responsibility mappings, multi-core execution logic, and build-time configuration matrices.

**Source credibility:** A specialized hardware project with active recent maintenance and decent community traction for its niche.

**Recency:** Highly current, incorporating very recent module additions and detailed SDK/PlatformIO instructions.

**Source:** [osemenyuk-114/zx-rgbi-to-vga-hdmi/CLAUDE.md](https://github.com/osemenyuk-114/zx-rgbi-to-vga-hdmi/blob/18b79607b0bc713d0d1d85c8841bf6395b9e843d/CLAUDE.md) · 20★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Project Context for AI Assistants

## Project Overview

**zx-rgbi-to-vga-hdmi** — Firmware for a Raspberry Pi Pico (RP2040) that converts ZX Spectrum RGBI video signals to VGA or HDMI (DVI) output.

- Upstream hardware reference: [ZX_RGBI2VGA-HDMI](https://github.com/AlexEkb4ever/ZX_RGBI2VGA-HDMI/)
- Native Pico SDK variant: [zx-rgbi-to-vga-hdmi-PICOSDK](https://github.com/osemenyuk-114/zx-rgbi-to-vga-hdmi-PICOSDK)
- Firmware version: `v1.7.2-dev` (see `ZX_RGBI_TO_VGA_HDMI/g_config.h`)

### New in v1.7.2-dev
- PS/2 keyboard support with PIO driver
- ZX Spectrum keyboard emulation via CH446Q analog switch
- Human-editable keyboard mapping table
- Conditional compilation for keyboard features

---

## Repository Structure

```
platformio.ini              # PlatformIO build config (environments, board, flags)
ZX_RGBI_TO_VGA_HDMI/        # Main firmware source
  ZX_RGBI_TO_VGA_HDMI.ino   # Arduino entry point (setup/loop)
  g_config.h                # Global config: board variants, feature flags, pin maps
  settings.h/.c             # Persistent settings (flash, CRC-32 validated)
  rgb_capture.h/.c          # PIO-based RGBI input capture
  video_output.h/.c         # VGA/
```

</details>
