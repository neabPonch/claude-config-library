---
name: rhysnewell__aviary__skill-in
source: https://github.com/rhysnewell/aviary/blob/396a742b4f6be7a3e3197cc778a8838438ed3591/docs/SKILL.md.in
repo: rhysnewell/aviary
kind: skill
stars: 107
last_pushed: 2026-06-12T04:45:19Z
license: gpl-3.0
score: 9
domains: [bioinformatics, cli-tools]
tags: [metagenomics, pipeline, genomics]
curated: 2026-06-16
curated_by: config-scout
---

# rhysnewell/aviary — skill

**Why it's worth keeping:** The use of dense, tabular CLI references and explicit environment variable mappings makes it a perfect knowledge base for an agent to generate complex, parameter-heavy commands. It clearly defines the dependencies between different biological workflow stages.

**Summary:** A highly structured operational manual for the Aviary metagenomics pipeline, covering installation, database configuration, and multi-stage execution.

**Source credibility:** High; specialized bioinformatics software with active maintenance and clear documentation standards.

**Recency:** Current; incorporates modern dependency management via Pixi alongside traditional methods.

**Source:** [rhysnewell/aviary/docs/SKILL.md.in](https://github.com/rhysnewell/aviary/blob/396a742b4f6be7a3e3197cc778a8838438ed3591/docs/SKILL.md.in) · 107★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Aviary

**Comprehensive Snakemake-based metagenomics pipeline: assembly → binning → annotation → dereplication.**
Supports short-read, long-read, and hybrid workflows. Each module runs independently or as a chained pipeline.

> **GitHub:** https://github.com/rhysnewell/aviary
> **Docs:** https://rhysnewell.github.io/aviary
> **Latest version:** [AVIARY_VERSION]


---

## 1. INSTALLATION

```bash
# Set conda channels first (required)
conda config --add channels defaults
conda config --add channels bioconda
conda config --add channels conda-forge

# Option A — Bioconda
conda create -n aviary -c bioconda aviary
# OR into an existing environment:
conda install -c bioconda aviary

# Option B — Pip (create environment from admin/requirements.txt first)
pip install aviary-genome

# Option C — Source with pixi (recommended for development)
git clone https://github.com/rhysnewell/aviary.git
cd aviary
pixi run postinstall     # installs all dependencies

# Editable install for development
pip install -e .
```


---

## 2. QUICK REFERENCE — SUBCOMMANDS

```bash
aviary --version            # show installed version
aviary --help               # top-level help
aviary <subcommand> --help  # hel
```

</details>
