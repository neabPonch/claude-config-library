---
name: ccattuto__esp-agentic-dev__claude
source: https://github.com/ccattuto/esp-agentic-dev/blob/a63f70b00e91dd5c3b27f20fd45cc9f0f3f8daf9/templates/CLAUDE.md
repo: ccattuto/esp-agentic-dev
kind: claude-md
stars: 6
last_pushed: 2026-04-21T10:27:28Z
license: mit
score: 9
domains: [embedded, iot-hardware, systems-programming]
tags: [esp32, jtag, rtt, firmware]
curated: 2026-06-15
curated_by: config-scout
---

# ccattuto/esp-agentic-dev — claude-md

**Why it's worth keeping:** It includes an architectural diagram of tool interactions and provides critical 'never guess' constraints to prevent LLM hallucinations in low-level register access.

**Summary:** This config establishes a highly specialized hardware-in-the-loop workflow using JTAG and RTT for ESP32 development.

**Source credibility:** High; the project shows deep niche expertise in embedded debug workflows with active maintenance.

**Recency:** Very recent (2 months ago), perfectly aligned with current agentic coding capabilities.

**Source:** [ccattuto/esp-agentic-dev/templates/CLAUDE.md](https://github.com/ccattuto/esp-agentic-dev/blob/a63f70b00e91dd5c3b27f20fd45cc9f0f3f8daf9/templates/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Agentic Firmware Development over JTAG

This project uses a pure-JTAG workflow for embedded firmware development.
No serial port is used at any point — flashing, log capture, and debugging
all go through OpenOCD's JTAG interface via USB.

## Configuration

Two configuration files control the tooling:

**`esp_target_config.json`** — project-level tooling setup:
- Which chip hardware description to use
- OpenOCD settings (board config, ports, flash command)
- Toolchain prefix (used to derive nm, objdump, addr2line, and default GDB)
- GDB executable (defaults to `{prefix}gdb` if not specified)
- Logging method (rtt or apptrace)

**`chips/<chip>.json`** — pure hardware reference (memory map, architecture).
Referenced by `esp_target_config.json`. Never needs editing per-project.
A chip JSON file may contain a reference to the corresponding SVD file with peripheral register definitions.

**`board.md`** — describes the specific development board: GPIO pin
assignments, I2C/SPI bus connections, LEDs (type, pin, protocol),
buttons, sensors, power domains, and any other hardware context
relevant to firmware development. Read this before writing any code
that interacts with board peripherals
```

</details>
