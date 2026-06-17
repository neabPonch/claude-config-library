---
name: cedbossneo__mowglinext
source: https://github.com/cedbossneo/mowglinext/blob/85d157a537fe9ec70ace989c0ea1acc9bb81aa98/CLAUDE.md
repo: cedbossneo/mowglinext
kind: claude-md
stars: 14
last_pushed: 2026-06-15T06:02:15Z
license: other
score: 10
domains: [robotics, embedded-systems]
tags: [ros2, autonomous-navigation, hardware-integration]
curated: 2026-06-15
curated_by: config-scout
---

# cedbossneo/mowglinext — claude-md

**Why it's worth keeping:** Uses 'Architecture Invariants' to establish hard constraints that prevent the AI from making destructive changes to physical behavior; provides granular cross-module dependency logic essential for high-stakes hardware integration.

**Summary:** Provides rigorous architectural invariants and safety protocols for a complex ROS2 autonomous robotics stack.

**Source credibility:** Extremely high technical depth regarding ROS2, GTSAM, and STM32 firmware with active maintenance history.

**Recency:** Highly current, referencing modern stacks like BehaviorTree.CPP v4 and recent development cycles.

**Source:** [cedbossneo/mowglinext/CLAUDE.md](https://github.com/cedbossneo/mowglinext/blob/85d157a537fe9ec70ace989c0ea1acc9bb81aa98/CLAUDE.md) · 14★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# MowgliNext

Open-source autonomous robot mower monorepo. ROS2 Kilted, Nav2, robot_localization (dual EKF: local wheel+gyro, global +GPS, under `two_d_mode`) — with an opt-in GTSAM iSAM2 factor-graph localizer (`fusion_graph`, in `ros2/src/fusion_graph/`) that 1-for-1 replaces `ekf_map_node` when `use_fusion_graph:=true` and adds optional LiDAR scan-matching + loop-closure factors. BehaviorTree.CPP v4, cell-based strip coverage. (`docs/HANDOFF_FUSION_GRAPH.md` is historical — kept around as the migration record but **not** the steady-state reference; see [`wiki/Architecture.md`](https://github.com/cedbossneo/mowglinext/wiki/Architecture#optional-factor-graph-localizer-fusion_graph) for current behaviour.)

**Website:** https://mowgli.garden | **Wiki:** https://github.com/cedbossneo/mowglinext/wiki | **First-boot checklist:** [`docs/FIRST_BOOT.md`](docs/FIRST_BOOT.md)

## Safety — READ FIRST

This robot has spinning blades. The STM32 firmware is the sole blade safety authority.

- NEVER bypass firmware blade safety checks from ROS2
- Blade commands from ROS2 are fire-and-forget — firmware decides whether to execute
- Emergency stop is handled by firmware, not software
- Flag ANY ch
```

</details>
