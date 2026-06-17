---
name: SmokinCaterpillar__pypet
source: https://github.com/SmokinCaterpillar/pypet/blob/a95aabf1ef4a3c8066495a0d10ee32d8c02600fe/CLAUDE.md
repo: SmokinCaterpillar/pypet
kind: claude-md
stars: 91
last_pushed: 2026-03-13T21:47:07Z
license: bsd-3-clause
score: 9
domains: [scientific-computing, python, data-science]
tags: [parameter-exploration, hdf5, technical-debt]
curated: 2026-06-14
curated_by: config-scout
---

# SmokinCaterpillar/pypet — claude-md

**Why it's worth keeping:** The 'Modernization Notes' explicitly detail technical debt, preventing the agent from repeating outdated patterns; the 'Architecture & Patterns' explains non-obvious internal logic like custom method prefixes.

**Summary:** Provides deep architectural context including specific naming conventions and a highly valuable 'Modernization Notes' section.

**Source credibility:** A specialized scientific tool with moderate GitHub popularity and clear authorship.

**Recency:** Contains explicit notes on what is outdated, making it highly relevant for modern maintenance tasks.

**Source:** [SmokinCaterpillar/pypet/CLAUDE.md](https://github.com/SmokinCaterpillar/pypet/blob/a95aabf1ef4a3c8066495a0d10ee32d8c02600fe/CLAUDE.md) · 91★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - pypet

## Project Overview

pypet (Python Parameter Exploration Toolkit) is a library for managing
numerical simulations with easy parameter exploration and HDF5 data
storage. Parameters and results are organized in a tree structure
called a **Trajectory**.

- **Version**: 0.6.1
- **License**: BSD
- **Author**: Robert Meyer
- **Python**: `>=3.6` (classifiers list 3.6-3.8; 3.6 and 3.7 are EOL)
- **Repo**: <https://github.com/SmokinCaterpillar/pypet>

## Project Structure

```text
pypet/                  # Main package
  environment.py        # Environment: top-level experiment runner
  trajectory.py         # Trajectory: tree container for params & results
  parameter.py          # Parameter types (Parameter, ArrayParameter, etc.)
  naturalnaming.py      # Natural naming / attribute access on tree nodes
  storageservice.py     # HDF5 storage via PyTables
  pypetconstants.py     # Constants and wrap modes
  pypetlogging.py       # Logging utilities, HasLogger mixin
  pypetexceptions.py    # Custom exception classes
  annotations.py        # WithAnnotations mixin
  slots.py              # HasSlots / MetaSlotMachine (__slots__ support)
  shareddata.py         # Shared dat
```

</details>
