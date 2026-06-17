---
name: iphands__HomeControl
source: https://github.com/iphands/HomeControl/blob/7670c6f51c1a1f1822fbe99633d8aa82a65b28ef/CLAUDE.md
repo: iphands/HomeControl
kind: claude-md
stars: 0
last_pushed: 2026-01-31T18:14:05Z
license: unknown
score: 8
domains: [embedded-systems, backend-api, systems-programming]
tags: [python, rust, esp32, protocol-specs, environment-guardrails]
curated: 2026-06-16
curated_by: config-scout
---

# iphands/HomeControl — claude-md

**Why it's worth keeping:** Includes high-value 'environmental intelligence' regarding container detection and venv constraints to prevent agentic errors in restricted environments.

**Summary:** Defines a dual-language (Python/Rust) architecture with specific UDP protocol specifications and parity requirements.

**Source credibility:** Low star count; likely an individual developer project.

**Recency:** Current; addresses modern deployment concerns like containerization and specific virtual environment management.

**Source:** [iphands/HomeControl/CLAUDE.md](https://github.com/iphands/HomeControl/blob/7670c6f51c1a1f1822fbe99633d8aa82a65b28ef/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# HomeCtrl - LED Controller System

## Overview

Networked LED strip animation system with Python and Rust server implementations, ESP32 firmware, and isolated external tests.

**Key principle**: Both server implementations must pass the same test suite to prove behavioral parity.

## Architecture

Three components:
1. **Server** - Python/Flask or Rust/Actix-web REST API + animation loop + UDP broadcasts
2. **Embedded Firmware** - ESP32/ESP8266 receives UDP, drives WS2811/WS2812 strips
3. **External Tests** - Standalone validation via REST API + UDP capture (no shared code with server)

## UDP Protocol

5-byte header + RGB data:
- Byte 0: Message type (1=LED_STRIP)
- Byte 1: Sequence (0-255)
- Byte 2: Brightness (0-255)
- Byte 3: LED count
- Byte 4: Device ID
- Bytes 5+: 3 bytes per LED (RGB)

Multi-strip support via device ID filtering.

## API Endpoints

| Endpoint | Purpose |
|----------|---------|
| `/api/modes` | List/set animation modes |
| `/api/brightness` | Get/set brightness |
| `/api/delay` | Get/set animation speed |
| `/api/opts` | Mode-specific options |
| `/api/strips` | Strip configuration |
| `/api/looper` | Loop control (debug mode only) |

## Debug Mode

`--debug
```

</details>
