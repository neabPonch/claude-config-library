---
name: beita6969__ScienceClaw__skill
source: https://github.com/beita6969/ScienceClaw/blob/7f5e65691672d5bc58c4615260b5e5f9b4ea7ee9/skills/chemistry/SKILL.md
repo: beita6969/ScienceClaw
kind: skill
stars: 846
last_pushed: 2026-06-08T13:27:28Z
license: mit
score: 8
domains: [science, chemistry, bioinformatics]
tags: [cheminformatics, drug-discovery, computational-chemistry]
curated: 2026-06-16
curated_by: config-scout
---

# beita6969/ScienceClaw — skill

**Why it's worth keeping:** The explicit, step-by-step procedure definitions (like Virtual Screening and QSAR modeling) provide the agent with clear logical blueprints for complex scientific tasks.

**Summary:** A highly structured domain-knowledge file for computational chemistry and drug discovery workflows.

**Source credibility:** Strong; high star count and recent activity indicate a reputable research-oriented toolset.

**Recency:** 

**Source:** [beita6969/ScienceClaw/skills/chemistry/SKILL.md](https://github.com/beita6969/ScienceClaw/blob/7f5e65691672d5bc58c4615260b5e5f9b4ea7ee9/skills/chemistry/SKILL.md) · 846★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: chemistry
description: # Chemistry & Drug Discovery
---

# Chemistry & Drug Discovery

## Overview
Computational chemistry, cheminformatics, and drug discovery workflows.

## Key Tools
- **RDKit**: Molecular manipulation, fingerprints, descriptors, substructure search
- **PubChem**: Chemical compound database (100M+ compounds)
- **ChEMBL**: Bioactivity database for drug-like molecules
- **Open Babel**: Format conversion, 3D generation
- **AutoDock Vina**: Molecular docking
- **GROMACS/OpenMM**: Molecular dynamics simulations

## Common Workflows

### Virtual Screening
1. Define target (protein structure from PDB)
2. Prepare compound library (from ChEMBL/ZINC/Enamine)
3. Filter by drug-likeness (Lipinski's Rule of Five)
4. Docking (AutoDock Vina, GNINA)
5. Scoring and ranking
6. ADMET prediction (absorption, distribution, metabolism, excretion, toxicity)
7. Hit validation

### QSAR Modeling
1. Curate activity data (ChEMBL IC50/Ki/EC50)
2. Calculate molecular descriptors (RDKit)
3. Feature selection
4. Model training (Random Forest, XGBoost, neural network)
5. Validation (cross-validation, external test set)
6. Applicability domain assessment

### Molecular Property Predict
```

</details>
