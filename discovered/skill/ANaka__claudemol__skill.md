---
name: ANaka__claudemol__skill
source: https://github.com/ANaka/claudemol/blob/7959ed8ef302d001f99cee89cc444068b86deb5d/claude-plugin/skills/rfd3/SKILL.md
repo: ANaka/claudemol
kind: skill
stars: 2
last_pushed: 2026-03-31T07:09:48Z
license: mit
score: 9
domains: [bioinformatics, scientific-workflows, structural-biology]
tags: [PyMOL, RFD3, protein-design, interactive-config]
curated: 2026-06-15
curated_by: config-scout
---

# ANaka/claudemol — skill

**Why it's worth keeping:** It provides highly specific domain constraints (e.g., forbidden JSON keys) and a structured 'Verify-Visualize-Confirm' loop that prevents tool-specific errors.

**Summary:** An interactive agent workflow for bridging PyMOL visualization with RFD3 protein design configuration generation.

**Source credibility:** Low star count but high technical density suggests it is a specialized research utility.

**Recency:** Recent; pushed within the last 2 months.

**Source:** [ANaka/claudemol/claude-plugin/skills/rfd3/SKILL.md](https://github.com/ANaka/claudemol/blob/7959ed8ef302d001f99cee89cc444068b86deb5d/claude-plugin/skills/rfd3/SKILL.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: rfd3
description: RFD3 Interactive Config Builder with PyMOL
version: 0.1.0
---

# RFD3 Interactive Config Builder with PyMOL

This document guides Claude Code + PyMOL (pymol-agent-bridge) through interactive construction and visualization of RFD3 protein design configurations.

## Prerequisites

- PyMOL running with the pymol-agent-bridge socket plugin (run `pymol-agent-bridge setup`)
- Structure file (PDB or CIF) to design around

## Quick Reference: Color Scheme

| Config Element | Color | Representation |
|---------------|-------|----------------|
| Fixed residues (motif) | cyan | sticks |
| Design regions | magenta | cartoon (transparent) |
| Ligand (RET) | yellow | spheres |
| Hotspots | red | spheres |
| Unindexed motifs | orange | sticks |
| Backbone only | marine | cartoon |
| Target protein (binder design) | gray | surface |
| ORI marker | green | sphere (large) |
| H-bond donors | blue | sticks |
| H-bond acceptors | red | sticks |


PyMOL one-liner:
```python
remove resn HOH+WAT+NA+CL+MG+CA+ZN+K+GOL+PEG+EDO+SO4+PO4+ACT+DMS
```

---

## Interactive Workflow

### Step 1: Load and Inspect Structure

```python
# Load structure
fetch 1ABC  # or: load /path/to/struc
```

</details>
