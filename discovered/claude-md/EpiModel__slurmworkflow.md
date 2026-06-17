---
name: EpiModel__slurmworkflow
source: https://github.com/EpiModel/slurmworkflow/blob/b13f81a0355df2f47d62f39375748326538c7047/CLAUDE.md
repo: EpiModel/slurmworkflow
kind: claude-md
stars: 2
last_pushed: 2026-03-30T14:29:37Z
license: other
score: 8
domains: [cli-tools, data-science, hpc]
tags: [R, Slurm, HPC, Workflow Management]
curated: 2026-06-15
curated_by: config-scout
---

# EpiModel/slurmworkflow — claude-md

**Why it's worth keeping:** Excellent use of 'Conventions' to enforce specific technical constraints (like long-form sbatch flags) and environment variable prefixes. It also provides concrete development commands that allow an agent to verify its work.

**Summary:** Provides a clear overview of an R package for Slurm HPC workflow management, including file mapping and development workflows.

**Source credibility:** The project is specialized with a clear author and follows modern R development standards.

**Recency:** Current; uses modern tools like testthat edition 3 and specific R version requirements.

**Source:** [EpiModel/slurmworkflow/CLAUDE.md](https://github.com/EpiModel/slurmworkflow/blob/b13f81a0355df2f47d62f39375748326538c7047/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — slurmworkflow

## Project Overview

**slurmworkflow** is an R package that builds and manages multi-step computational workflows on Slurm-equipped HPC systems. It chains `sbatch` jobs via `--dependency=afterany` so users don't need persistent SSH sessions or long-lived daemons.

- **Author:** Adrien Le Guillou
- **License:** MIT
- **Version:** 0.1.0
- **R requirement:** >= 4.1.0
- **Hard dependencies:** `fs`, `yaml`
- **Docs site:** https://epimodel.github.io/slurmworkflow/

## Repository Structure

```
R/                    # Package source
  workflow.R          # Core API: create_workflow, add_workflow_step, load_workflow, etc.
  step_templates.R    # All step_tmpl_* functions and helpers
  sbatch_options.R    # Sbatch option validation (150+ valid options)
  wf_summary.R        # Workflow YAML I/O
  dir.R               # Directory creation and template copying
  env-vars.R          # Environment variable mapping
  utils.R             # Template variable substitution (simple_brew)
inst/
  templates/          # Bash/R template files copied into workflow directories
tests/testthat/       # Comprehensive test suite
vignettes/            # Main vignette: slurmworkflow.R
```

</details>
