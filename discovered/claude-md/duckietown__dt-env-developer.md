---
name: duckietown__dt-env-developer
source: https://github.com/duckietown/dt-env-developer/blob/618ac818d360792335648c19729a448bd9db53f9/CLAUDE.md
repo: duckietown/dt-env-developer
kind: claude-md
stars: 3
last_pushed: 2026-06-08T13:49:58Z
license: unknown
score: 9
domains: [robotics, embedded-systems, ros]
tags: [robotics, ros, docker, hardware]
curated: 2026-06-14
curated_by: config-scout
---

# duckietown/dt-env-developer — claude-md

**Why it's worth keeping:** Includes highly specific code templates for class inheritance (DTROS), strict naming conventions (sub_/pub_/cb_), and clear rules against hardcoded parameters that are critical for an LLM to follow in a robotics context.

**Summary:** Provides comprehensive instructions for the Duckietown robotics platform, covering tool-specific CLI commands, project structure, and mandatory ROS node patterns.

**Source credibility:** High; comes from a structured, well-documented hardware/software ecosystem with active development.

**Recency:** Current; reflects modern Docker and ROS development workflows.

**Source:** [duckietown/dt-env-developer/CLAUDE.md](https://github.com/duckietown/dt-env-developer/blob/618ac818d360792335648c19729a448bd9db53f9/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Duckietown Developer Guide for Claude

## Project Overview

Duckietown is a robotics development platform for:
- **Duckiebots** — ground-based autonomous vehicles
- **Duckiedrones** — aerial vehicles (DD21, DD24)

All code runs inside Docker containers using the **DTProject** standard. Primary tooling: Duckietown Shell (`dts`), Docker, ROS Noetic.

---

## Key Commands

```bash
# Discover robots on the network
dts fleet discover

# Build image locally (force rebuild)
dts devel build -f

# Build directly on a robot
dts devel build -f -H ROBOT_NAME

# Run locally
dts devel run

# Run on a robot with a specific launcher
dts devel run -H ROBOT_NAME -L launcher_name
```

Robots are accessible via `ROBOT_NAME.local` hostname resolution.

---

## DTProject Structure

```
my-project/
├── .dtproject              # Marks repo as a Duckietown Project (required)
├── Dockerfile              # ARG REPO_NAME, DESCRIPTION, MAINTAINER (fill placeholders)
├── configurations.yaml     # Docker container run configurations
├── packages/               # Python and Catkin packages
│   └── my_package/
│       ├── __init__.py
│       ├── src/            # ROS nodes (node files here)
│       ├── launch/
```

</details>
