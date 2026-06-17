---
name: Hugues-DTANKOUO__scientific-pdf-translator
source: https://github.com/Hugues-DTANKOUO/scientific-pdf-translator/blob/317ef40f6090f4b769de2cb984a63c9af8cd4dc2/CLAUDE.md
repo: Hugues-DTANKOUO/scientific-pdf-translator
kind: claude-md
stars: 12
last_pushed: 2026-03-11T01:25:45Z
license: other
score: 9
domains: [document-processing, agents-ai, workflows]
tags: [ocr, translation, latex, state-management]
curated: 2026-06-16
curated_by: config-scout
---

# Hugues-DTANKOUO/scientific-pdf-translator — claude-md

**Why it's worth keeping:** It implements a robust 'checkpoint' pattern using TODO.md for interruption recovery and enforces quality through explicit visual verification steps between OCR output and original images.

**Summary:** A highly structured, multi-phase workflow for translating complex scientific PDFs using OCR and LaTeX.

**Source credibility:** Specialized tool with hand-crafted, high-logic orchestration instructions.

**Recency:** Extremely relevant for modern agentic workflows requiring state management over long-running tasks.

**Source:** [Hugues-DTANKOUO/scientific-pdf-translator/CLAUDE.md](https://github.com/Hugues-DTANKOUO/scientific-pdf-translator/blob/317ef40f6090f4b769de2cb984a63c9af8cd4dc2/CLAUDE.md) · 12★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Instructions for Claude - Scientific PDF Translation

## 🎯 Your Mission

You are about to help translate a scientific PDF document from English to French. This is a quality-focused task that requires patience, precision, and attention to detail. The goal is to produce a professionally formatted, accurately translated document that maintains the academic rigor of the original.

## 📋 Initial Setup

### Step 1: Create TODO.md
**FIRST AND FOREMOST**: Create a comprehensive TODO.md file that lists EVERY step of this process. This file will be your checkpoint system. Make it exhaustive - include every single task, no matter how small.

### Step 2: Python Environment
Create and activate a Python virtual environment with Python 3.11+:
```bash
python3.11 -m venv venv
source venv/bin/activate  # On macOS/Linux
```

**CRITICAL**: Use this virtual environment for ALL Python operations throughout this process.

### Step 3: Check System Requirements

1. **Tesseract OCR**: 
   - Check if installed: `which tesseract`
   - If not installed, ask the user to run: `./scripts/install_macos.sh`
   - Or install manually: `brew install tesseract`

2. **MacTeX**:
   - Check if installed: `which pdflatex`
```

</details>
