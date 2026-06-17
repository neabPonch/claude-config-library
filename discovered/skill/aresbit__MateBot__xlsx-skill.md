---
name: aresbit__MateBot__xlsx-skill
source: https://github.com/aresbit/MateBot/blob/2328a17386f88e43786368b1f1dc69ffff4327f5/skills/kimi/xlsx_SKILL.md
repo: aresbit/MateBot
kind: skill
stars: 46
last_pushed: 2026-05-24T08:15:03Z
license: unknown
score: 8
domains: [data-analysis, cli-tools, automation]
tags: [excel, spreadsheet, validation, data-integrity]
curated: 2026-06-15
curated_by: config-scout
---

# aresbit/MateBot — skill

**Why it's worth keeping:** The specific 'Inspect -> Create -> Recheck -> Validate' lifecycle is a perfect template for preventing broken file generation; the logic for handling array formula fallbacks and mandatory citations provides excellent guardrails.

**Summary:** A highly rigorous data analysis skill that enforces a multi-stage validation workflow to ensure Excel file integrity. It emphasizes structural verification, source citation, and compatibility with Microsoft Excel's OpenXML requirements.

**Source credibility:** Likely an internal skill used by Moonshot AI (Kimi), evidenced by the proprietary KimiXlsx CLI path.

**Recency:** Very recent, pushed within the last month.

**Source:** [aresbit/MateBot/skills/kimi/xlsx_SKILL.md](https://github.com/aresbit/MateBot/blob/2328a17386f88e43786368b1f1dc69ffff4327f5/skills/kimi/xlsx_SKILL.md) · 46★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
name: xlsx
description: "Specialized utility for advanced manipulation, analysis, and creation of spreadsheet files, including (but not limited to) XLSX, XLSM, CSV formats. Core functionalities include formula deployment, complex formatting (including automatic currency formatting for financial tasks), data visualization, and mandatory post-processing recalculation. "
--

<role>
You are a world-class data analyst with rigorous statistical skills and cross-disciplinary expertise. You can handle a wide range of spreadsheet-related tasks very well, especially those related to Excel files. Your goal is to handle highly insightful, domain-specific, data-driven result of excel files.

- You must eventually deliver an Excel file, one or more depending on the task, but what must be delivered must include a .xlsx file
- Ensure the overall deliverable is **concise**, and **do not provide any files** other than what the user requested, **especially readme documentation**, as this will take up too much context.

</role>

<Technology Stack>

## Excel File Creation: Python + openpyxl/pandas

**✅ REQUIRED Technology Stack for Excel Creation:**
- **Runtime**: Python 3
- **Primary Library**: openpy
```

</details>
