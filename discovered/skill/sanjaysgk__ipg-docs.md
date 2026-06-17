---
name: sanjaysgk__ipg-docs
source: https://github.com/sanjaysgk/ipg-docs/blob/94446ff306f26d6b4e6ffb71559df8bec920eaf5/skill.md
repo: sanjaysgk/ipg-docs
kind: skill
stars: 0
last_pushed: 2026-04-09T05:10:10Z
license: mit
score: 8
domains: [bioinformatics, cli-tools, science]
tags: [nextflow, genomics, hpc]
curated: 2026-06-15
curated_by: config-scout
---

# sanjaysgk/ipg-docs — skill

**Why it's worth keeping:** The structure transitions from high-level capabilities to actionable 'Skills' (CLI commands) and real-world 'Workflows' (test, production, adaptation), teaching the agent how to reason through complex task scenarios.

**Summary:** Provides comprehensive operational knowledge for a specific Nextflow bioinformatics pipeline, covering installation, execution profiles, and subworkflow mappings.

**Source credibility:** Highly credible; includes specific academic citations, nf-core standards, and detailed technical specifications.

**Recency:** Current; references recent Nextflow versions and modern containerization engines.

**Source:** [sanjaysgk/ipg-docs/skill.md](https://github.com/sanjaysgk/ipg-docs/blob/94446ff306f26d6b4e6ffb71559df8bec920eaf5/skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ipg
description: Build and document the sanjaysgk/ipg nf-core Nextflow pipeline for cryptic peptide database construction from RNA-seq data. Use when running the pipeline, looking up parameters, debugging errors, citing the work, or extending it.
license: MIT
compatibility: Requires Nextflow ≥ 24.04.2 and a container engine (Docker, Singularity, Podman, Apptainer, or Conda fallback). Tested on Monash M3 SLURM with Singularity.
metadata:
  author: sanjaysgk
  version: "0.1-dev"
  paper: "10.1016/j.mcpro.2021.100143"
---

# IPG: Immunopeptidogenomics cryptic peptide pipeline

This skill describes how an AI agent can work with the IPG documentation site to help users install, run, debug, cite, and extend the `sanjaysgk/ipg` nf-core pipeline.

## What IPG does

`sanjaysgk/ipg` is a Nextflow DSL2 pipeline that consumes paired-end RNA-seq reads and produces a sample-specific three-frame translated protein FASTA database for searching tandem mass spectrometry spectra. The deliverable, `<sample>_cryptic.fasta`, lets researchers identify cryptic peptides — translation products that aren't in standard reference proteomes. The pipeline implements 31 steps from a legacy bash script g
```

</details>
