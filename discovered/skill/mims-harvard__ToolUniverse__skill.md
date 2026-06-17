---
name: mims-harvard__ToolUniverse__skill
source: https://github.com/mims-harvard/ToolUniverse/blob/7d6a182fda817c84da9f4441d8d40bee3a0bcc9c/skills/tooluniverse-electron-microscopy/SKILL.md
repo: mims-harvard/ToolUniverse
kind: skill
stars: 1450
last_pushed: 2026-06-14T23:49:43Z
license: apache-2.0
score: 9
domains: [scientific-research, data-analysis]
tags: [microscopy, workflow-automation, structural-biology]
curated: 2026-06-15
curated_by: config-scout
---

# mims-harvard/ToolUniverse — skill

**Why it's worth keeping:** Features elite meta-instructions like 'Compute, Don't Describe' and domain-specific heuristics (e.g., resolution thresholds) that are easily transferable to any technical agent role.

**Summary:** A highly structured research skill that navigates the full lifecycle of electron microscopy data, from raw datasets to validated atomic models.

**Source credibility:** High; produced by a reputable Harvard MIMS research group with significant community validation.

**Recency:** Current; utilizes modern tool-use, multi-phase reasoning, and structured query parsing patterns.

**Source:** [mims-harvard/ToolUniverse/skills/tooluniverse-electron-microscopy/SKILL.md](https://github.com/mims-harvard/ToolUniverse/blob/7d6a182fda817c84da9f4441d8d40bee3a0bcc9c/skills/tooluniverse-electron-microscopy/SKILL.md) · 1450★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: tooluniverse-electron-microscopy
description: Search and analyze electron microscopy data — cryo-EM density maps (EMDB), fitted atomic models (PDB), raw micrograph datasets (EMPIAR), and cryo-electron tomography volumes (CryoET Data Portal). Use for finding 3D structural data on a protein/complex, comparing experimental EM resolution to AlphaFold confidence, and accessing raw EM data for re-processing.
disable-model-invocation: true
---

# Electron Microscopy Structure Analysis

Pipeline for discovering and analyzing electron microscopy data across the full resolution spectrum: from 3D density maps (EMDB) to fitted atomic models (PDB), raw micrograph datasets (EMPIAR), and cryo-electron tomography volumes (CryoET Data Portal). Connects EM data to structural biology context via PDB and AlphaFold.

**Guiding principles**:
1. **Resolution awareness** -- always report and interpret map resolution; sub-4A enables atomic modeling, 4-8A enables domain fitting, >8A is shape-level
2. **Map before model** -- the density map is the primary experimental data; fitted models are interpretations
3. **Method matters** -- single particle analysis, tomography, 2D crystallography, and helic
```

</details>
