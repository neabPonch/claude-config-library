---
name: Shock-Nin__MyTool
source: https://github.com/Shock-Nin/MyTool/blob/3f5cfee48e9ee540ac567c18be6234a9c105b2e5/CLAUDE.MD
repo: Shock-Nin/MyTool
kind: claude-md
stars: 0
last_pushed: 2026-05-30T02:32:58Z
license: unknown
score: 9
domains: [python, automation, desktop-app, cross-platform]
tags: [architecture, design-patterns, coding-standards]
curated: 2026-06-14
curated_by: config-scout
---

# Shock-Nin/MyTool — claude-md

**Why it's worth keeping:** It explicitly defines a non-standard naming convention (snake_case modules to PascalCase classes) and catalogs existing utility functions to prevent the AI from reinventing them. The inclusion of security warnings and environmental configuration logic provides vital context for safe coding.

**Summary:** An excellent project-specific guide that maps out complex architectural patterns like dynamic module loading and platform-specific logic. It includes highly actionable 'DO/DON'T' sections tailored to the codebase's specific quirks.

**Source credibility:** Low public credibility due to 0 stars/no description, but represents a high-quality internal documentation standard.

**Recency:** Highly current; utilizes modern 'Do/Don't' prompting structures ideal for Claude Code and agentic workflows.

**Source:** [Shock-Nin/MyTool/CLAUDE.MD](https://github.com/Shock-Nin/MyTool/blob/3f5cfee48e9ee540ac567c18be6234a9c105b2e5/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# MyTool - Claude Code Documentation

## Project Overview

MyTool is a Python-based integrated toolset for Windows and Mac environments, providing a GUI application for various business operations including:

- **Trading & Analysis**: Anomaly detection, EA (Expert Advisor) testing, predictive modeling (ARIMA, RNN, Keras)
- **Asset Management**: Personal asset tracking, financial data processing
- **Web Automation**: Automated web login, data scraping
- **Platform Utilities**: Display management, alert timers, dictionary tools

## Architecture

### Entry Points

- **mytool.py**: Main GUI application using FreeSimpleGUI
  - Provides menu-driven interface for all tools
  - Supports password-protected login
  - Multi-platform support (Windows/Mac)

- **run.py**: Command-line module executor
  - Dynamic module loading using importlib
  - Converts snake_case module names to PascalCase class names
  - Pattern: `python run.py -m <module> -e <event>`

- **batch.py**: Batch processing executor

### Directory Structure

```
MyTool/
├── business/          # Business logic modules
│   ├── mac/          # Mac-specific features
│   ├── windows/      # Windows-specific features
│   ├── predict/
```

</details>
