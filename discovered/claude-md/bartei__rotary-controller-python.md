---
name: bartei__rotary-controller-python
source: https://github.com/bartei/rotary-controller-python/blob/a953127625817fc0df49aee9ad96971785e385f3/CLAUDE.md
repo: bartei/rotary-controller-python
kind: claude-md
stars: 82
last_pushed: 2026-05-07T04:00:15Z
license: unknown
score: 9
domains: [embedded-systems, python, ui-frameworks]
tags: [kivy, modbus, hardware-control]
curated: 2026-06-15
curated_by: config-scout
---

# bartei/rotary-controller-python — claude-md

**Why it's worth keeping:** Includes explicit 'Component Patterns' and code snippets for known pain points like circular dependencies, ensuring new modules adhere to the specific architectural boilerplate.

**Summary:** A highly detailed instruction set for a Kivy-based hardware control project that bridges high-level UI logic with low-level embedded communication.

**Source credibility:** High; 82 stars and very recent maintenance suggest a real-world, used tool.

**Recency:** Modern; uses current industry standards like `uv` and Python 3.10+ syntax.

**Source:** [bartei/rotary-controller-python/CLAUDE.md](https://github.com/bartei/rotary-controller-python/blob/a953127625817fc0df49aee9ad96971785e385f3/CLAUDE.md) · 82★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Project Standards for RCP (Rotary Controller Python)

## Project Overview

RCP is a Kivy-based DRO (Digital Read-Out) and single-axis controller UI for rotary tables.
It communicates with embedded hardware (STM32) over RS-485/Modbus RTU using `minimalmodbus`.
Target platforms: Raspberry Pi (primary), Linux, Windows, macOS.

## Build and Run

```bash
# Install dependencies
uv sync

# Run the application
uv run python -m rcp.main

# Run tests
uv run pytest

# Build package
uv build
```

## Project Structure

```
rcp/
├── main.py                    # Entry point (asyncio + Kivy event loop)
├── app.py                     # MainApp class (Kivy App)
├── feeds.py                   # Feed/thread pitch configurations (Pydantic models)
├── components/                # UI layer
│   ├── manager.py             # ScreenManager (navigation)
│   ├── appsettings.py         # ConfigParser setup
│   ├── home/                  # Home screen components (coordbar, servobar, elsbar, jogbar, statusbar)
│   ├── screens/               # Full-screen views (home, setup, scale, servo, formats, network, update, color_picker)
│   ├── plot/                  # Plot/visualization (scene, circle_popup,
```

</details>
