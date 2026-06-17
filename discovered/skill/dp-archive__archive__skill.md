---
name: dp-archive__archive__skill
source: https://github.com/dp-archive/archive/blob/f8bf8cab697714b02956d2d363631e4ee9547927/seed_skills/rdkit/SKILL.md
repo: dp-archive/archive
kind: skill
stars: 1103
last_pushed: 2026-03-04T08:01:19Z
license: apache-2.0
score: 9
domains: [science, data-analysis, python]
tags: [rdkit, cheminformatics, molecular-analysis]
curated: 2026-06-16
curated_by: config-scout
---

# dp-archive/archive — skill

**Why it's worth keeping:** Uses modern RDKit generator APIs rather than deprecated ones and includes critical error-handling logic like None-type checks after parsing.

**Summary:** Provides highly specific RDKit API patterns for molecular I/O, sanitization, descriptors, and similarity calculations.

**Source credibility:** High; structured as a professional tool-use specification with clear technical depth.

**Recency:** 

**Source:** [dp-archive/archive/seed_skills/rdkit/SKILL.md](https://github.com/dp-archive/archive/blob/f8bf8cab697714b02956d2d363631e4ee9547927/seed_skills/rdkit/SKILL.md) · 1103★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: rdkit
description: Cheminformatics toolkit for fine-grained molecular control. SMILES/SDF parsing, descriptors (MW, LogP, TPSA), fingerprints, substructure search, 2D/3D generation, similarity, reactions. For standard workflows with simpler interface, use datamol (wrapper around RDKit). Use rdkit for advanced control, custom sanitization, specialized algorithms.
license: BSD-3-Clause license
metadata:
    skill-author: K-Dense Inc.
---

# RDKit Cheminformatics Toolkit

## Overview

RDKit is a comprehensive cheminformatics library providing Python APIs for molecular analysis and manipulation. This skill provides guidance for reading/writing molecular structures, calculating descriptors, fingerprinting, substructure searching, chemical reactions, 2D/3D coordinate generation, and molecular visualization. Use this skill for drug discovery, computational chemistry, and cheminformatics research tasks.

## Core Capabilities

### 1. Molecular I/O and Creation

**Reading Molecules:**

Read molecular structures from various formats:

```python
from rdkit import Chem

# From SMILES strings
mol = Chem.MolFromSmiles('Cc1ccccc1')  # Returns Mol object or None

# From MOL files
mol = Ch
```

</details>
