---
name: Vadim-GSADUs__GSADUs.Revit.Addin
source: https://github.com/Vadim-GSADUs/GSADUs.Revit.Addin/blob/d4be73b6ba14b70961177077e9109f42200baa45/CLAUDE.MD
repo: Vadim-GSADUs/GSADUs.Revit.Addin
kind: claude-md
stars: 0
last_pushed: 2026-03-04T18:26:31Z
license: unknown
score: 9
domains: [.net, desktop-apps, bim-software]
tags: [architecture-mapping, technical-debt-tracking, line-number-references]
curated: 2026-06-14
curated_by: config-scout
---

# Vadim-GSADUs/GSADUs.Revit.Addin — claude-md

**Why it's worth keeping:** Includes specific line number references for entry points/core logic and an explicit list of technical debt to prevent the AI from assuming code is clean.

**Summary:** A high-density guide that provides mapping of critical logic via file line numbers and detailed architectural rationale.

**Source credibility:** Single-developer niche tool with highly professional, documentation-first approach.

**Recency:** Extremely current, targeting .NET 8 and Revit 2026.

**Source:** [Vadim-GSADUs/GSADUs.Revit.Addin/CLAUDE.MD](https://github.com/Vadim-GSADUs/GSADUs.Revit.Addin/blob/d4be73b6ba14b70961177077e9109f42200baa45/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.MD - AI Assistant Guide

## Project Overview

**GSADUs Revit Batch Export Add-in** is a Revit 2026 add-in that provides batch export capabilities for selection sets with advanced curation, staging, and multi-format export workflows (PDF, images, RVT, CSV).

## Technology Stack

- **Platform**: .NET 8.0 (Windows)
- **UI Framework**: WPF
- **Target Application**: Autodesk Revit 2026
- **Architecture**: Dependency Injection (Microsoft.Extensions.DependencyInjection)
- **Language**: C# (latest version, nullable reference types enabled)

## Project Structure

```
GSADUs.Revit.BatchExport.sln
└── src/GSADUs.Revit.Addin/
    ├── Abstractions/       # Interface definitions for core services
    ├── Commands/           # Revit external commands
    ├── Curate/            # Ambiguity visualization logic
    ├── Domain/            # Domain models and audit caching
    ├── Infrastructure/     # Concrete implementations, adapters, DI setup
    ├── Logging/           # CSV batch logging, performance logging
    ├── Orchestration/     # Batch run coordination
    ├── UI/                # WPF windows, view models, converters
    ├── Workflows/         # Export action implementations (PDF,
```

</details>
