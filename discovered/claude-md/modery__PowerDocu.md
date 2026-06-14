---
name: modery__PowerDocu
source: https://github.com/modery/PowerDocu/blob/779f67278578899e0501c6da40ed2a0b40aa19f1/CLAUDE.md
repo: modery/PowerDocu
kind: claude-md
stars: 625
last_pushed: 2026-06-14T09:13:03Z
license: mit
score: 9
domains: [dotnet, cli-tools, automation]
tags: [architecture-guide, submodule-awareness, pipeline-logic]
curated: 2026-06-14
curated_by: config-scout
---

# modery/PowerDocu — claude-md

**Why it's worth keeping:** The breakdown of submodule entity/parser classes and the explicit description of the two-phase execution pipeline are elite techniques for guiding LLMs through large codebases.

**Summary:** This file provides a highly detailed architectural roadmap of a complex .NET solution, including the internal contents of its Git submodules.

**Source credibility:** Highly credible; 625 stars indicates significant community adoption and active development.

**Recency:** Extremely current, referencing .NET 10 and modern dependency versions.

**Source:** [modery/PowerDocu/CLAUDE.md](https://github.com/modery/PowerDocu/blob/779f67278578899e0501c6da40ed2a0b40aa19f1/CLAUDE.md) · 625★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — PowerDocu Codebase Guide

## Project Overview

PowerDocu is a .NET 10 Windows application that auto-generates technical documentation for Microsoft Power Platform components (Cloud Flows, Canvas Apps, Model-Driven Apps, Copilot Studio Agents, AI Models, Business Process Flows, Desktop Flows, and Solutions). Output formats are **Word (.docx)**, **Markdown (.md)**, and **HTML**.

The application ships as a **Windows GUI** (`PowerDocu.exe`) and also supports a **CLI** interface via command-line flags.

---

## Repository Structure

```
PowerDocu/
├── PowerDocu.sln                      # Visual Studio solution (all projects)
├── modules/
│   └── PowerDocu.Common/              # Git submodule (https://github.com/modery/PowerDocu.Common)
│       └── PowerDocu.Common/          # The actual library project
├── PowerDocu.GUI/                     # Entry point: WinForms GUI + CLI runner
├── PowerDocu.SolutionDocumenter/      # Orchestrator for .zip solution packages
├── PowerDocu.FlowDocumenter/          # Cloud Flow documentation
├── PowerDocu.AppDocumenter/           # Canvas App documentation
├── PowerDocu.AgentDocumenter/         # Copilot Studio Agent documentation
├── Pow
```

</details>
