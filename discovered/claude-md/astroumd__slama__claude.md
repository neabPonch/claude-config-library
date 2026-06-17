---
name: astroumd__slama__claude
source: https://github.com/astroumd/slama/blob/813a345a766ef4d334c602eb4237862241821591/slama/CLAUDE.md
repo: astroumd/slama
kind: claude-md
stars: 3
last_pushed: 2026-06-10T14:22:56Z
license: mit
score: 9
domains: [web-backend, science-computing, observatory-systems]
tags: [architecture-diagrams, data-flow, simulations, uv-package-manager, fastapi]
curated: 2026-06-16
curated_by: config-scout
---

# astroumd/slama — claude-md

**Why it's worth keeping:** It includes critical 'gotchas' like threading requirements for synchronous libraries and a command to simulate real-world data, enabling the agent to verify its work via simulation.

**Summary:** Provides an exceptionally detailed technical map including data flow diagrams, specific class responsibilities, and domain-specific context.

**Source credibility:** High; authored by developers working on actual observatory instrumentation with high recent activity.

**Recency:** Current; uses modern tooling like `uv` and provides specific instructions for local development/simulation.

**Source:** [astroumd/slama/slama/CLAUDE.md](https://github.com/astroumd/slama/blob/813a345a766ef4d334c602eb4237862241821591/slama/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Background

The Submillimeter Array (SMA) is a collection of 8 radiotelescopes working
in tandem as an interferometer.  The SMA observes in the millimeter and
submillimiter wavelength bands. The SMA is located at the summit of Mauna
Kea in Hawaii.

## Project Overview

**SLAMA** (SMA LMA code) is a Python package for a web-based monitoring
system for the SMA observatory instruments, similar to CARMA's monitor
system.  It reads/writes monitor point data via an SMAX (SMA Extended)
server backed by Redis/Valkey on `localhost:6380`, and serves live
telemetry to browsers via FastAPI + HTMX + Jinja2. Users can browse
subsystem displays and click any numeric cell for an interactive time
series plot.

## Commands

**Install (development mode)**:
```bash
cd slama
uv sync
uv pip install -e .
```

**Run the web server**:
```bash
uv run uvicorn slama.web.server:app --reload --port 8000
```
Then open `http://localhost:8000/`.

**Simulate observatory data** (in a separate terminal, with SMAX running):
```bash
cd src/slama
uv run fakeobs.py
```

**Tests**: the legacy `test/` cod
```

</details>
