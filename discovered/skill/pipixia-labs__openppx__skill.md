---
name: pipixia-labs__openppx__skill
source: https://github.com/pipixia-labs/openppx/blob/18bbdd9ecf9b7624c32a700455de17013717c55a/openppx/skills/opencv/SKILL.md
repo: pipixia-labs/openppx
kind: skill
stars: 10
last_pushed: 2026-06-10T09:12:22Z
license: apache-2.0
score: 9
domains: [computer-vision, image-processing]
tags: [opencv, cv2, python, video]
curated: 2026-06-15
curated_by: config-scout
---

# pipixia-labs/openppx — skill

**Why it's worth keeping:** The 'Guardrails' section is exceptional, proactively solving common agent failures like BGR/RGB color space confusion and unclosed video captures. It also provides a robust debugging strategy of saving intermediate files to trace pipeline failures.

**Summary:** A highly specialized skill for deterministic image and video processing using OpenCV in Python.

**Source credibility:** High-quality technical depth suggests an expert author despite low repository star count.

**Recency:** 

**Source:** [pipixia-labs/openppx/openppx/skills/opencv/SKILL.md](https://github.com/pipixia-labs/openppx/blob/18bbdd9ecf9b7624c32a700455de17013717c55a/openppx/skills/opencv/SKILL.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: opencv
description: Use OpenCV for Python image processing, contour analysis, thresholding, filtering, geometric transforms, and basic video I/O. Trigger when the user asks to process images or video with cv2/OpenCV, or when a task clearly fits classical computer vision instead of a remote VLM.
---

# OpenCV

Use this skill when the user wants local computer-vision work with OpenCV, especially:

- image filtering, thresholding, morphology, contours, or edge detection
- resize, crop, rotate, perspective transform, or format conversion
- camera or video frame read/write with `cv2.VideoCapture` or `cv2.VideoWriter`
- classical vision pipelines that should run locally in Python

Prefer this skill for deterministic image processing. If the task is mainly semantic understanding, captioning, or open-ended visual reasoning, consider an image-understanding expert instead of forcing OpenCV.

## Workflow

1. Confirm the real task type first: image enhancement, segmentation, contour extraction, geometry transform, or video I/O.
2. Start with the smallest reproducible pipeline and save intermediate outputs when debugging.
3. Use Python and import OpenCV as `cv2 as cv` unless the surro
```

</details>
