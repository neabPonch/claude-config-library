---
name: mrzzmrzz__BioSkill__skill
source: https://github.com/mrzzmrzz/BioSkill/blob/5c73b56b07cce950dd23a62740da339b445234e1/src/skills/af3-structure-json/SKILL.md
repo: mrzzmrzz/BioSkill
kind: skill
stars: 3
last_pushed: 2026-02-16T15:16:09Z
license: mit
score: 8
domains: [bioinformatics, cli-tools, scientific-computing]
tags: [alphafold3, pdb, mmcif, structural-biology]
curated: 2026-06-15
curated_by: config-scout
---

# mrzzmrzz/BioSkill — skill

**Why it's worth keeping:** Includes precise CLI usage, strict output guarantees, and detailed troubleshooting steps that allow an agent to handle scientific edge cases autonomously.

**Summary:** Provides instructions for converting PDB/mmCIF structural data into validated AlphaFold3 JSON formats, including ligand and sequence extraction.

**Source credibility:** Low star count (3), but the technical depth implies a highly specialized bioinformatics utility.

**Recency:** Very recent; aligns with current AlphaFold3 research workflows.

**Source:** [mrzzmrzz/BioSkill/src/skills/af3-structure-json/SKILL.md](https://github.com/mrzzmrzz/BioSkill/blob/5c73b56b07cce950dd23a62740da339b445234e1/src/skills/af3-structure-json/SKILL.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: af3-structure-json
description: Convert a single PDB/mmCIF structure into a validated AlphaFold3 JSON (alphafold3 dialect) by extracting polymer sequences, PTM/base modifications, ligands or ions (CCD codes), and optional bondedAtomPairs. Use when AF3 inputs must be rebuilt from solved structures while preserving chemistry.
---

# PDB/mmCIF Structure -> AlphaFold3 JSON

Generate one AlphaFold3 (AF3) input JSON per structure file.

Use this skill when solved structures already exist in PDB/mmCIF and AF3 input must preserve:
- polymer sequences rebuilt from coordinates,
- non-canonical residues/bases as `modifications`,
- ligands/ions as AF3 `ligand` entities,
- optional covalent links as `bondedAtomPairs`.

Reference spec: `references/AlphaFold3_input.md`.

## Quick run

1. Prepare input:
- Prefer **mmCIF** if covalent links matter (`struct_conn` is richer than PDB CONECT).
- Keep one biological assembly/model per file for predictable entity extraction.

2. Convert:

```bash
.venv/bin/python skills/af3-structure-json/scripts/structure_to_af3_json.py --help

.venv/bin/python skills/af3-structure-json/scripts/structure_to_af3_json.py \
  -i complex.cif \
  -o runs/$(date +%Y
```

</details>
