---
name: matlab__matlab-agentic-toolkit__skill
source: https://github.com/matlab/matlab-agentic-toolkit/blob/002f5d04ba19772de0e5cead5a56501064eeaa34/skills-catalog/signal-processing/matlab-configure-scope-object/SKILL.md
repo: matlab/matlab-agentic-toolkit
kind: skill
stars: 623
last_pushed: 2026-06-04T15:49:26Z
license: other
score: 9
domains: [scientific-computing, agents-ai, safety-engineering]
tags: [boundary-enforcement, error-handling, api-safety, matlab]
curated: 2026-06-15
curated_by: config-scout
---

# matlab/matlab-agentic-toolkit — skill

**Why it's worth keeping:** Demonstrates an advanced 'Safety Boundary' pattern using explicit whitelists and a structured verification workflow (List -> Confirm -> Set). The robust error handling/retry logic is highly transferable to any high-stakes API interaction.

**Summary:** Prevents MATLAB/Simulink crashes by restricting agent access to documented public APIs for scope objects. It enforces a strict boundary between user-facing properties and internal framework implementation details.

**Source credibility:** Professional grade; authored by MathWorks for their official agentic toolkit.

**Recency:** 

**Source:** [matlab/matlab-agentic-toolkit/skills-catalog/signal-processing/matlab-configure-scope-object/SKILL.md](https://github.com/matlab/matlab-agentic-toolkit/blob/002f5d04ba19772de0e5cead5a56501064eeaa34/skills-catalog/signal-processing/matlab-configure-scope-object/SKILL.md) · 623★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: matlab-configure-scope-object
description: Prevents crashes due to problematic scope-related API misuse caused by agent escalation into internal scope framework objects. Use when configuring properties of scope-related Simulink blocks or MATLAB objects — constrains the agent to documented APIs and directs users to the scope UI when a property is not programmatically accessible.
license: MathWorks BSD-3-Clause
metadata:
  author: MathWorks
  version: "1.0"
---

# Scope Configuration — Safe API Skill

## When To Use

This skill is active whenever you interact with properties of any scope-related block or object:

**Simulink blocks:**
- Scope, Floating Scope (Simulink)
- Time Scope, Spectrum Analyzer, Array Plot (DSP System Toolbox)
- Constellation Diagram, Eye Diagram (Communications Toolbox)
- Video Viewer (Computer Vision Toolbox)
- Point Cloud Viewer (Point Cloud Toolbox)
- Scope Viewer (signal-level viewer)
- Range-Time Intensity Scope, Angle-Time Intensity Scope, Doppler-Time Intensity Scope (Phased Array System Toolbox)

**MATLAB objects:**
- `timescope(...)` 
- `spectrumAnalyzer(...)` (formerly `dsp.SpectrumAnalyzer`)
- `dsp.ArrayPlot(...)`
- `comm.ConstellationDiagr
```

</details>
