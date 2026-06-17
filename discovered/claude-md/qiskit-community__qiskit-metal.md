---
name: qiskit-community__qiskit-metal
source: https://github.com/qiskit-community/qiskit-metal/blob/dda578901ebdde1ad1eb7d64a812d1e8779ce163/CLAUDE.md
repo: qiskit-community/qiskit-metal
kind: claude-md
stars: 409
last_pushed: 2026-06-14T20:10:00Z
license: apache-2.0
score: 10
domains: [scientific-computing, python]
tags: [architecture-mapping, risk-mitigation, workflow-specialization]
curated: 2026-06-15
curated_by: config-scout
---

# qiskit-community/qiskit-metal — claude-md

**Why it's worth keeping:** The 'Hard constraints' pattern is a masterclass in risk mitigation for hardware-interfacing code, and the use of specific context pointers (.claude/context/) facilitates an advanced multi-file knowledge hierarchy.

**Summary:** Provides a high-density architectural map and defines high-risk 'hard touch' zones to prevent destructive changes in specialized environments. It also clarifies complex, non-obvious project workflows like the dual-folder synchronization requirement.

**Source credibility:** Very high; from a significant and actively maintained quantum computing framework.

**Recency:** Extremely current, referencing modern tooling like `uv` and Python 3.12.

**Source:** [qiskit-community/qiskit-metal/CLAUDE.md](https://github.com/qiskit-community/qiskit-metal/blob/dda578901ebdde1ad1eb7d64a812d1e8779ce163/CLAUDE.md) · 409★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Quantum Metal repo guide for AI agents

> If you are a Claude (or other AI agent) opening this repo for the first
> time, **read this file end-to-end before touching anything**. It points
> at the rest of the context that will save you hours.

## What this repo is

**Quantum Metal** (formerly Qiskit Metal) is an open-source Python framework
for designing and analysing superconducting quantum chips. The PyPI package
is `quantum-metal`; the import path is still `qiskit_metal` for backward
compatibility. The community-maintained successor to IBM's original
Qiskit Metal — the rebrand is in progress through the v0.6.x line.

Stack: Python 3.10–3.12 · `shapely` for geometry · `geopandas` /
`pandas` for storage · `matplotlib` for headless viewing · `PySide6` for
the optional desktop GUI · `pyEPR-quantum` / `pyaedt` / `gmsh` /
`Elmer` for analysis backends.

## Architecture map (skim these first)

| Path | What lives there |
|------|------------------|
| `src/qiskit_metal/qlibrary/` | All `QComponent` subclasses (transmons, terminations, lumped, couplers, routes, sample shapes). The user-visible catalogue. |
| `src/qiskit_metal/qlibrary/core/base.py` | `QComponent` — the load
```

</details>
