---
name: kevinlawrenceking__court-beta
source: https://github.com/kevinlawrenceking/court-beta/blob/c3158e9572d17b0b1d0c9d2802926f15ab43ad8b/CLAUDE.md
repo: kevinlawrenceking/court-beta
kind: claude-md
stars: 0
last_pushed: 2026-03-12T01:04:05Z
license: unknown
score: 9
domains: [backend-api, ai-agents, data-processing]
tags: [cfml, python, gemini-ai, ocr]
curated: 2026-06-15
curated_by: config-scout
---

# kevinlawrenceking/court-beta — claude-md

**Why it's worth keeping:** It includes practical 'Common Development Patterns' (code snippets) that enforce security and consistency in legacy environments, plus precise instructions on the multi-step AI logic to prevent hallucinations.

**Summary:** A highly detailed guide for a legal monitoring system involving ColdFusion, Python, and Gemini AI. It provides deep architectural context and specific implementation patterns.

**Source credibility:** While the repo has low visibility, the content is highly specific, containing production-grade paths and specialized business logic.

**Recency:** Very current; includes modern tech like Python 3.12 and latest Gemini models.

**Source:** [kevinlawrenceking/court-beta/CLAUDE.md](https://github.com/kevinlawrenceking/court-beta/blob/c3158e9572d17b0b1d0c9d2802926f15ab43ad8b/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

DocketWatch is a court case monitoring and AI-powered legal document summarization system built for TMZ. It tracks celebrity-related legal cases, monitors PACER RSS feeds, and generates newsworthy summaries of legal documents using AI.

**Technology Stack:**
- **Backend:** ColdFusion (CFML) on Windows Server
- **Database:** Microsoft SQL Server (datasource: "Reach", database: "docketwatch")
- **Frontend:** Bootstrap 5, jQuery, DataTables
- **Python:** 3.12+ for PDF processing, OCR, and AI summarization
- **AI:** Google Gemini API (gemini-2.5-flash, gemini-2.5-pro)

## Development Commands

### ColdFusion Development
- **No build process required** - CFML is interpreted at runtime
- **Test changes:** Save `.cfm` files and refresh browser (restart CF application if needed)
- **View logs:** Check ColdFusion Administrator logs and custom logs (written via `cflog`)

### Python Scripts
```bash
# Test PDF processing
python U:\docketwatch\python\combined_pacer_pdf_processor.py <url> <output_path>

# Test AI summarization (ad-hoc upload tool)
python U:\do
```

</details>
