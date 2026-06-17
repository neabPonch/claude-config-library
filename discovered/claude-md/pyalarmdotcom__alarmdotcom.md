---
name: pyalarmdotcom__alarmdotcom
source: https://github.com/pyalarmdotcom/alarmdotcom/blob/4d817516c4a20315fb586741277db12289da1586/CLAUDE.md
repo: pyalarmdotcom/alarmdotcom
kind: claude-md
stars: 164
last_pushed: 2026-04-22T07:33:19Z
license: mit
score: 9
domains: [iot, backend]
tags: [architecture, workflow, python, home-assistant]
curated: 2026-06-16
curated_by: config-scout
---

# pyalarmdotcom/alarmdotcom — claude-md

**Why it's worth keeping:** The 'Data Flow' and 'Common Workflows' sections are exceptional; they transform abstract code into actionable logical steps that an AI can use to implement new features or debug.

**Summary:** Provides a deep architectural breakdown of a Home Assistant integration, mapping out specific data flows and dependency relationships.

**Source credibility:** Active niche project with 164 stars and recent maintenance (2 months ago).

**Recency:** Very current, utilizing modern standards like Ruff, MyPy, and pre-commit hooks.

**Source:** [pyalarmdotcom/alarmdotcom/CLAUDE.md](https://github.com/pyalarmdotcom/alarmdotcom/blob/4d817516c4a20315fb586741277db12289da1586/CLAUDE.md) · 164★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an unofficial Home Assistant custom component that integrates Alarm.com security systems and devices. The integration communicates with Alarm.com's unofficial web API via the `pyalarmdotcomajax` library. It supports alarm panels, sensors, locks, lights, garage doors, thermostats, and other Alarm.com-connected devices.

**Important**: This is a safety-critical integration. Changes must be thoroughly tested and never rely on untested code for security functions.

## Code Architecture

### Component Structure

The integration follows Home Assistant's standard custom component architecture:

- **`custom_components/alarmdotcom/`**: Main integration directory
  - **`__init__.py`**: Integration setup, config entry management, and config entry migrations (v1→v5)
  - **`hub.py`**: Core controller (`AlarmHub`) that manages the pyalarmdotcomajax `AlarmBridge` API connection and WebSocket event monitoring
  - **`entity.py`**: Base classes for all Alarm.com entities
    - `AdcEntity`: Generic base entity with pub/sub event handling
    - `AdcEntityDes
```

</details>
