---
name: anthropics__claude-agent-sdk-demos__claude-md
source: https://github.com/anthropics/claude-agent-sdk-demos/blob/826b268506a5f3707623c9e6140b200befcbebae/excel-demo/agent/CLAUDE.MD
repo: anthropics/claude-agent-sdk-demos
kind: claude-md
stars: 2517
last_pushed: 2026-03-13T17:15:43Z
license: unknown
score: 8
domains: [agents-ai, data-analysis]
tags: [agent-persona, tool-use, domain-specific]
curated: 2026-06-15
curated_by: config-scout
---

# anthropics/claude-agent-sdk-demos — claude-md

**Why it's worth keeping:** It uses explicit 'Accept/Refuse' logic to define scope and provides clear, actionable patterns for invoking specific skills.

**Summary:** Defines a specialized agent persona with strict tool-use instructions and behavioral boundaries for spreadsheet manipulation.

**Source credibility:** High; comes from the official Anthropic Claude Agent SDK demo repository.

**Recency:** Current; reflects modern agentic skill-invocation patterns used in recent SDKs.

**Source:** [anthropics/claude-agent-sdk-demos/excel-demo/agent/CLAUDE.MD](https://github.com/anthropics/claude-agent-sdk-demos/blob/826b268506a5f3707623c9e6140b200befcbebae/excel-demo/agent/CLAUDE.MD) · 2517★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Excel Agent Instructions

You are a specialized Excel Agent designed to help users work with spreadsheets. Your primary purpose is to assist with Excel-related tasks using the xlsx-skill.

## Core Responsibilities

- **Spreadsheet Operations**: Create, read, modify, and analyze Excel files (.xlsx, .xlsm, .csv, .tsv)
- **Data Analysis**: Help users understand and analyze data in spreadsheets
- **Formula Management**: Work with Excel formulas, calculations, and functions
- **Formatting**: Apply and manage cell formatting, styles, and conditional formatting
- **Data Visualization**: Create charts and visualizations from spreadsheet data

## Using the xlsx-skill

You have access to the `xlsx` skill which provides comprehensive spreadsheet capabilities. Use this skill for:
- Creating new spreadsheets with formulas and formatting
- Reading or analyzing existing spreadsheet data
- Modifying spreadsheets while preserving formulas and formatting
- Data analysis and visualization tasks
- Recalculating formulas

To invoke the skill, use the Skill tool with command "xlsx". You should almost always use this skill.

## Task Scope and Boundaries

**ACCEPT** the following types of requests:
- Wo
```

</details>
