---
name: elkimek__get-based
source: https://github.com/elkimek/get-based/blob/74269b788d86d02be34525eb2db1e1b8555410ff/CLAUDE.md
repo: elkimek/get-based
kind: claude-md
stars: 78
last_pushed: 2026-06-15T06:35:30Z
license: agpl-3.0
score: 9
domains: [web-frontend, health-tech]
tags: [module-mapping, architecture-heavy, no-build-system]
curated: 2026-06-15
curated_by: config-scout
---

# elkimek/get-based — claude-md

**Why it's worth keeping:** The file excels by grouping files by concern rather than just listing them, explaining the specific role each module plays in the startup/runtime lifecycle. It also explicitly defines technical constraints (like the lack of a build system) to prevent tool-chain hallucinations.

**Summary:** Provides a highly detailed functional map of an ESM-only architecture and deep domain context for a complex health data application.

**Source credibility:** High; a specialized, active project with significant architectural depth.

**Recency:** Very current; reflects modern ESM-only patterns and contemporary AI integration workflows.

**Source:** [elkimek/get-based/CLAUDE.md](https://github.com/elkimek/get-based/blob/74269b788d86d02be34525eb2db1e1b8555410ff/CLAUDE.md) · 78★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

getbased is a personal health intelligence platform organized around five lenses on the user's biology — **Labs**, **Genome**, **Body**, **Light**, **Insight**. Every lens informs every other: DNA shapes how labs are interpreted, wearable physiology shapes which biomarkers matter most, light environment shapes sleep and hormones, and the AI synthesizes across all of them with full context. Anti-reductionist by design.

- **🩸 Labs**: biomarkers across 17 categories + 217 specialty markers (custom marker pipeline), AI-powered PDF import, biological age (PhenoAge + Bortz), trend detection, correlation viewer
- **🧬 Genome**: 51 curated SNPs, APOE haplotype, 39 mtDNA haplogroups, DNA-aware recommendations
- **⌚ Body**: 7 wearable vendors (Oura/Withings/Ultrahuman/WHOOP/Fitbit/Polar/Apple Health), manual biometrics, cycle tracking with phase-aware ranges, EMF assessment (Baubiologie SBM-2015)
- **☀ Light**: sun sessions with Bird-Riordan spectral reconstruction, 19-preset photobiology device library (Chroma, EMR-Tek, Mitochondriak; custom devices suppo
```

</details>
