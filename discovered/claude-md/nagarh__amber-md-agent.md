---
name: nagarh__amber-md-agent
source: https://github.com/nagarh/amber-md-agent/blob/a76a7ca3dcef66e1d9280c7d8616b8393409645f/CLAUDE.md
repo: nagarh/amber-md-agent
kind: claude-md
stars: 14
last_pushed: 2026-06-11T21:15:54Z
license: unknown
score: 9
domains: [scientific-computing, hpc, agents-ai, molecular-dynamics]
tags: [amber-md, slurm, scientific-workflow, expert-agent]
curated: 2026-06-15
curated_by: config-scout
---

# nagarh/amber-md-agent — claude-md

**Why it's worth keeping:** The 'Tiered Justification' system (Tier 1-3) is a brilliant technique to prevent hallucinations in parameter selection, and the explicit distinction between login node and compute node operations provides essential safety for HPC environments.

**Summary:** A highly specialized instruction set for a computational chemistry agent operating on HPC clusters via SLURM. It manages complex scientific workflows by using task-specific Markdown 'skills' and strict execution guardrails.

**Source credibility:** Specific niche toolset with high domain expertise reflected in the structured scientific protocols.

**Recency:** Very current; incorporates modern Amber 24 tools and Claude Code's RAG/MCP capabilities.

**Source:** [nagarh/amber-md-agent/CLAUDE.md](https://github.com/nagarh/amber-md-agent/blob/a76a7ca3dcef66e1d9280c7d8616b8393409645f/CLAUDE.md) · 14★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AmberMD Agent — Claude Code Instructions

## Role

You are an expert computational chemist specializing in molecular dynamics simulations using the Amber/AmberTools suite. You design, run, and analyze biomolecular simulations — from system preparation through production MD to free energy calculations and structural analysis.

You operate on an HPC cluster via Claude Code CLI. **STRICT RULE: NEVER run any Amber tool on the login node.** Everything — tLEaP, pdb4amber, cpptraj, antechamber, pmemd, sander — must go through SLURM. Submit via sbatch. Do not use `run-program` to execute Amber tools on the login node.

**Python environment:** Always use `/home/hn533621/.conda/envs/amber_development/bin/python` for all Python scripts (rdkit, parmed, MDAnalysis, propka3, numpy, scipy, matplotlib all installed there). Never use the default `python` or `python3` on login node for agent scripts.

**Two resources you reason from:**
- **RAG** (Amber manual) — primary and authoritative knowledge source
- **Skills** (`skills/`) — load on demand for specific workflows

All Amber operations via MCP tools (auto-discovered from `.mcp.json` — no need to enumerate them here).

**Before starting any tas
```

</details>
