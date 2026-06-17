---
name: cggos__vins_mono_cg
source: https://github.com/cggos/vins_mono_cg/blob/dbd28e7a0e485a506c818d57c87c928a5a4400cc/CLAUDE.md
repo: cggos/vins_mono_cg
kind: claude-md
stars: 118
last_pushed: 2026-05-08T09:59:22Z
license: gpl-3.0
score: 9
domains: [robotics, computer-vision, cpp]
tags: [ros, vio, architecture-map, pipeline]
curated: 2026-06-15
curated_by: config-scout
---

# cggos/vins_mono_cg — claude-md

**Why it's worth keeping:** The architectural breakdown mapping specific files to their logical roles in the pipeline is exactly what an AI needs to navigate large C++ codebases without losing context.

**Summary:** A high-density technical guide for a complex ROS-based computer vision system, covering build commands, data pipelines, and evaluation workflows.

**Source credibility:** Derived from a highly-regarded robotics research project (VINS-Mono).

**Recency:** Highly relevant; provides a perfect template for documenting complex, multi-package dependencies and data flows.

**Source:** [cggos/vins_mono_cg/CLAUDE.md](https://github.com/cggos/vins_mono_cg/blob/dbd28e7a0e485a506c818d57c87c928a5a4400cc/CLAUDE.md) · 118★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

**vins_mono_cg** is a modified version of [VINS-Mono](https://github.com/HKUST-Aerial-Robotics/VINS-Mono) — a monocular visual-inertial odometry (VIO) system using an optimization-based sliding window formulator. It is a ROS-based C++11 project.

Dependencies: ROS (Kinetic/Melodic), Eigen 3.3.3, Ceres Solver, OpenCV, Boost.

## Build & Run

```sh
# From workspace root (ws_vins/)
catkin_make -j2
# or
catkin build

# Run with EuRoC dataset
roslaunch vins_estimator euroc.launch
rosbag play <PATH>/MH_01_easy.bag

# Docker build/run
cd docker && make build
./run.sh euroc.launch
```

## Code Formatting

```sh
./batch_format.sh   # runs clang-format -style=file on all .cpp/.h/.cu/.c files
```

## Package Architecture

The system is composed of four ROS packages that form a pipeline:

```
camera (image) ──→ feature_tracker ──→ vins_estimator ──→ pose_graph
IMU data ─────────────────────────────────────────────↗
```

### `camera_model`
A shared library (not a node) providing camera model abstractions used by `feature_tracker`:
- Models: `PinholeCamera`, `CataCame
```

</details>
