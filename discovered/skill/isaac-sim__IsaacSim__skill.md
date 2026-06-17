---
name: isaac-sim__IsaacSim__skill
source: https://github.com/isaac-sim/IsaacSim/blob/40316786340b3f034a229d9e12650df1ac0b68ab/skills/isaac-sim-remote/SKILL.md
repo: isaac-sim/IsaacSim
kind: skill
stars: 3468
last_pushed: 2026-06-04T22:08:55Z
license: other
score: 9
domains: [robotics, simulation, remote-control]
tags: [nvidia, isaac-sim, python-server, tcp]
curated: 2026-06-15
curated_by: config-scout
---

# isaac-sim/IsaacSim — skill

**Why it's worth keeping:** It provides robust patterns for connectivity verification (port polling), state isolation through named execution contexts, and advanced async task handling using a JSON envelope.

**Summary:** A specialized protocol for an agent to control a running NVIDIA Isaac Sim instance via a Python TCP server.

**Source credibility:** High; sourced from the official NVIDIA Isaac-Sim repository.

**Recency:** Current; reflects modern remote-execution/socket interaction workflows.

**Source:** [isaac-sim/IsaacSim/skills/isaac-sim-remote/SKILL.md](https://github.com/isaac-sim/IsaacSim/blob/40316786340b3f034a229d9e12650df1ac0b68ab/skills/isaac-sim-remote/SKILL.md) · 3468★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: isaac-sim-remote
description: >
  Connect to a running Isaac Sim via the `isaacsim.code_editor.python_server`
  TCP socket (port 8226) to execute Python remotely. Launch Isaac Sim, send
  code, create/modify USD stages, run simulations, take viewport or full-app
  screenshots, inspect/modify prims, control the camera, step physics, read
  console logs, execute Kit commands. Works in `--no-window` headless mode.
---

# Isaac Sim Remote

Execute Python inside a running Isaac Sim via the `isaacsim.code_editor.python_server` TCP socket.

Related: `debug-with-local-kit` (when behavior depends on a Kit-from-source build), `profile-isaac-sim` (to attach Tracy to the running process), `isaac-sim-validator` (final QA gate on any rendered output).

Upstream `isaac-sim-ui` (menu/widget OmniUIQuery automation) and `isaac-sim-recording` (cursor tracking, tutorial video capture) are not imported. The inline UI patterns here (Play-button click via `OmniUIQuery`, full-app vs viewport screenshots) cover the common cases.

## Launching Isaac Sim

```bash
cd _build/linux-x86_64/release

# Headless — supports all features: code execution, viewport screenshots,
# full-app screenshots, menu cl
```

</details>
