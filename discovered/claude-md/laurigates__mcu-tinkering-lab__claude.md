---
name: laurigates__mcu-tinkering-lab__claude
source: https://github.com/laurigates/mcu-tinkering-lab/blob/3b6aa1ad23141b679ebda9448c1ca56cea0c80ef/packages/robocar/simulation/CLAUDE.md
repo: laurigates/mcu-tinkering-lab
kind: claude-md
stars: 6
last_pushed: 2026-06-12T16:53:52Z
license: mit
score: 9
domains: [robotics, embedded-systems, simulation]
tags: [physics-engine, esp32, python, just-runner]
curated: 2026-06-15
curated_by: config-scout
---

# laurigates/mcu-tinkering-lab — claude-md

**Why it's worth keeping:** The inclusion of a module purpose table, data flow diagram, and exact byte-level protocol specifications provides high-context guidance for hardware-adjacent coding. Including current test failure rates is an excellent way to communicate system reliability to the agent.

**Summary:** A highly structured technical guide for an ESP32-based robotics physics simulation. It provides clear command references, architectural mapping, and specific communication protocols.

**Source credibility:** High; well-maintained repository with recent activity and specialized subject matter.

**Recency:** Current; leverages modern Python tooling like `uv` and `ruff`.

**Source:** [laurigates/mcu-tinkering-lab/packages/robocar/simulation/CLAUDE.md](https://github.com/laurigates/mcu-tinkering-lab/blob/3b6aa1ad23141b679ebda9448c1ca56cea0c80ef/packages/robocar/simulation/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — robocar-simulation

Python physics simulation environment for an ESP32-based differential drive robot car.

## Quick Reference

```bash
just --list          # All available recipes
just run             # Headless simulation
just run-visual      # GUI window (matplotlib)
just run-browser     # Browser-based (http://localhost:52000)
just test            # Run test suite
just lint            # Ruff check
just format          # Ruff format
just type-check      # ty (astral)
```

**Package manager**: `uv` (primary). Use `uv run <cmd>` for one-off commands. Run `uv sync --extra dev` to install dev dependencies.

**Entry point**: `src/main.py` → `SimulationManager`

---

## Architecture

### Core Modules (`src/`)

| Module | Purpose |
|--------|---------|
| `main.py` | `SimulationManager` — async coordination, CLI, signal handling |
| `robot_model.py` | `DifferentialDriveRobot`, `DCMotor`, `PhysicsEngine` (Pymunk) |
| `motor_controller.py` | PID control, encoder simulation, velocity filtering |
| `communication_bridge.py` | WebSocket/Serial/I2C protocol server |
| `genesis_visualizer.py` | Genesis 3D visualization (with Matplotlib 2D fallback when genesis-world is unavailabl
```

</details>
