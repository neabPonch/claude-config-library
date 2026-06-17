---
name: quekster__go2_stairs
source: https://github.com/quekster/go2_stairs/blob/9f821417a67eab70ed0e58190e37e2c7d567b9b6/Claude.md
repo: quekster/go2_stairs
kind: claude-md
stars: 1
last_pushed: 2026-04-22T10:33:50Z
license: unknown
score: 8
domains: [robotics, reinforcement-learning]
tags: [ppo, isaac-sim, quadruped, simulation]
curated: 2026-06-16
curated_by: config-scout
---

# quekster/go2_stairs — claude-md

**Why it's worth keeping:** It maps high-level research objectives to specific implementation files (e.g., mapping rewards to `rewards.py`) and explains mathematical nuances like LiDAR normalization that are critical for AI reasoning about physics-based code.

**Summary:** A highly detailed technical specification for training a quadruped robot via reinforcement learning in IsaacSim. It outlines complex curriculum phases, sensor processing, and reward-shaping logic.

**Source credibility:** Single-star academic/research project; depth of technical detail implies a legitimate, specialized codebase rather than boilerplate.

**Recency:** Very current, referencing recent IsaacSim 5.0 and IsaacLab 2.2 stacks.

**Source:** [quekster/go2_stairs/Claude.md](https://github.com/quekster/go2_stairs/blob/9f821417a67eab70ed0e58190e37e2c7d567b9b6/Claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# **Project: PPO-Based Stair Traversal for Unitree Go2 Using IsaacSim 5.0.0 + IsaacLab 2.2.0**

This project implements a **DirectRLEnv-based reinforcement learning pipeline** to train a **Unitree Go2** quadruped robot to **ascend (and later descend) custom stair terrains** using PPO.
A **LiDAR ray-based terrain perception module** guides the policy, producing a **non-blind, perception-aware controller**.

The project follows a **three-phase curriculum**, and all implementation details—including environment logic, reward shaping, termination functions, and LiDAR processing—are included below.

---

# **1. System Overview**

### **Simulation Stack**

* **IsaacSim 5.0.0**
* **IsaacLab 2.2.0**
* Custom project built using the *IsaacLab External Project Generator*:
  [https://isaac-sim.github.io/IsaacLab/main/source/overview/own-project/template.html](https://isaac-sim.github.io/IsaacLab/main/source/overview/own-project/template.html)

### **Goal**

Train a robust locomotion policy that:

1. **Ascends stairs** of various geometries (height, width, #steps).
2. Uses **LiDAR-based height estimation** to shape stable, terrain-aware locomotion.
3. Optionally **descends** stairs using contin
```

</details>
