---
name: laurenvil__Uno-QClaw__skill
source: https://github.com/laurenvil/Uno-QClaw/blob/8404c77524462e1c41c46c53e6e43b0c4561b587/workspace/skills/bridge/SKILL.md
repo: laurenvil/Uno-QClaw
kind: skill
stars: 17
last_pushed: 2026-06-10T04:41:11Z
license: mit
score: 9
domains: [embedded-systems, hardware-integration, iot]
tags: [rpc, inter-processor, arduino, linux]
curated: 2026-06-15
curated_by: config-scout
---

# laurenvil/Uno-QClaw — skill

**Why it's worth keeping:** It includes high-density technical constraints like latency expectations, mandatory initialization steps (Bridge.begin()), and specific 'don't use' scenarios that prevent agent errors. This prevents common integration failures when generating code for dual-processor systems.

**Summary:** Defines the RPC communication protocol between the Linux-side MPU and the Arduino-side MCU for the Uno Q hardware platform. It provides essential architectural constraints and usage patterns for cross-processor interaction.

**Source credibility:** High relevance to the specific Uno Q hardware with very recent activity.

**Recency:** Extremely current, pushed within the last month.

**Source:** [laurenvil/Uno-QClaw/workspace/skills/bridge/SKILL.md](https://github.com/laurenvil/Uno-QClaw/blob/8404c77524462e1c41c46c53e6e43b0c4561b587/workspace/skills/bridge/SKILL.md) · 17★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: bridge
description: Arduino Bridge — software RPC layer that connects Python on the MPU (Linux side) with Arduino sketches on the MCU (STM32U585). Read this BEFORE writing any project that combines a Python program with an Arduino sketch, or that asks "how do I send data from my sketch to the Linux side?". The Uno Q is two processors on one board; Bridge is how they talk.
---

# Bridge — Inter-Processor RPC on the Uno Q

The Arduino Uno Q is **two computers on one board**:

- **MPU** (Qualcomm QRB2210, 4× Cortex-A53 @ 2.0 GHz, Debian Linux) — runs Python, web servers, AI models, OpenCV.
- **MCU** (STMicroelectronics STM32U585, Cortex-M33 @ 160 MHz, Zephyr + Arduino Core) — runs `.ino` sketches, controls every Arduino header pin (digital I/O, PWM, ADC, I²C, SPI, UART, CAN).

**Bridge** is Arduino's software-based **Remote Procedure Call (RPC)** layer that lets either side call functions on the other:

```
Python (Linux side)                Arduino sketch (MCU side)
─────────────────                  ─────────────────────────
from bridge import ...             #include <Bridge.h>
result = bridge.call("read_A0")    Bridge.begin();
print(result)                      // expose
```

</details>
