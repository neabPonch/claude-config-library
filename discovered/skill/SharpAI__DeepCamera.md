---
name: SharpAI__DeepCamera
source: https://github.com/SharpAI/DeepCamera/blob/2264fcb20e545a8bc5b41097494e93b776104bf3/SKILL.md
repo: SharpAI/DeepCamera
kind: skill
stars: 2827
last_pushed: 2026-04-21T19:30:51Z
license: mit
score: 8
domains: [agents-ai, computer-vision, security]
tags: [depth-estimation, privacy, real-time-video, protocol-design]
curated: 2026-06-14
curated_by: config-scout
---

# SharpAI/DeepCamera — skill

**Why it's worth keeping:** It provides a professional blueprint for a JSONL-based stdin/stdout communication protocol and a clear inheritance pattern for implementing complex agentic capabilities.

**Summary:** A highly structured skill definition for real-time depth estimation used in privacy-focused camera surveillance.

**Source credibility:** High; the source repository is a popular (2.8k stars) and active AI computer vision project.

**Recency:** Current; features modern models like Depth Anything v2 and up-to-date hardware acceleration profiles.

**Source:** [SharpAI/DeepCamera/SKILL.md](https://github.com/SharpAI/DeepCamera/blob/2264fcb20e545a8bc5b41097494e93b776104bf3/SKILL.md) · 2827★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: depth-estimation
description: "Real-time depth map privacy transforms using Depth Anything v2 (CoreML + PyTorch)"
version: 1.2.0
category: privacy

parameters:
  - name: model
    label: "Depth Model"
    type: select
    options: ["depth-anything-v2-small", "depth-anything-v2-base", "depth-anything-v2-large"]
    default: "depth-anything-v2-small"
    group: Model

  - name: variant
    label: "CoreML Variant (macOS)"
    type: select
    options: ["DepthAnythingV2SmallF16", "DepthAnythingV2SmallF16INT8", "DepthAnythingV2SmallF32"]
    default: "DepthAnythingV2SmallF16"
    group: Model

  - name: blend_mode
    label: "Display Mode"
    type: select
    options: ["depth_only", "overlay", "side_by_side"]
    default: "depth_only"
    group: Display

  - name: opacity
    label: "Overlay Opacity"
    type: number
    min: 0.0
    max: 1.0
    default: 0.5
    group: Display

  - name: colormap
    label: "Depth Colormap"
    type: select
    options: ["inferno", "viridis", "plasma", "magma", "jet", "turbo", "hot", "cool"]
    default: "viridis"
    group: Display

  - name: device
    label: "Device"
    type: select
    options: ["auto", "cpu", "cuda", "mps"]
    default
```

</details>
