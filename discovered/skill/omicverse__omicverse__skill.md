---
name: omicverse__omicverse__skill
source: https://github.com/omicverse/omicverse/blob/58b8ca8fe48116648ddc8db71b6be217ec55d9dc/.claude/skills/data-export-excel/SKILL.md
repo: omicverse/omicverse
kind: skill
stars: 1034
last_pushed: 2026-06-14T09:03:14Z
license: gpl-3.0
score: 8
domains: [data-analysis, python-automation]
tags: [excel, formatting, data-science, openpyxl]
curated: 2026-06-16
curated_by: config-scout
---

# omicverse/omicverse — skill

**Why it's worth keeping:** It provides specific logic for high-value tasks like auto-adjusting column widths, header styling, and conditional formatting that standard pandas exports lack.

**Summary:** A procedural template for creating professional, styled Excel workbooks using openpyxl.

**Source credibility:** High; sourced from omicverse, a highly-regarded bioinformatics library.

**Recency:** 

**Source:** [omicverse/omicverse/.claude/skills/data-export-excel/SKILL.md](https://github.com/omicverse/omicverse/blob/58b8ca8fe48116648ddc8db71b6be217ec55d9dc/.claude/skills/data-export-excel/SKILL.md) · 1034★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: data-export-excel
title: Excel Data Export (Universal)
description: Export analysis results, data tables, and formatted spreadsheets to Excel files using openpyxl. Works with ANY LLM provider (GPT, Gemini, Claude, etc.).
---

# Excel Data Export (Universal)

## Overview
This skill enables you to export bioinformatics data, analysis results, and formatted tables to professional Excel spreadsheets. Unlike cloud-hosted solutions, this skill uses the **openpyxl** Python library and executes **locally** in your environment, making it compatible with **ALL LLM providers** including GPT, Gemini, Claude, DeepSeek, and Qwen.

## When to Use This Skill
- Export AnnData observations (.obs) or variables (.var) to Excel
- Save DEG analysis results with formatting
- Create multi-sheet workbooks with different data types
- Generate formatted Excel reports with cell styling
- Export cluster annotations, cell type assignments, or quality control metrics

## How to Use

### Step 1: Import Required Libraries
```python
import openpyxl
from openpyxl import Workbook
from openpyxl.styles import Font, PatternFill, Alignment, Border, Side
from openpyxl.utils.dataframe import dataframe_to_rows
imp
```

</details>
