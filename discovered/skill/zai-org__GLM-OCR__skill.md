---
name: zai-org__GLM-OCR__skill
source: https://github.com/zai-org/GLM-OCR/blob/cef4d0ea120d1741f5cefe8985eee45f6c8eff1d/skills/sdk/SKILL.md
repo: zai-org/GLM-OCR
kind: skill
stars: 6963
last_pushed: 2026-04-21T08:52:11Z
license: apache-2.0
score: 9
domains: [agents-ai, cli-tools, document-processing, ocr]
tags: [OCR, SDK, Structured-Data, CLI]
curated: 2026-06-14
curated_by: config-scout
---

# zai-org/GLM-OCR — skill

**Why it's worth keeping:** Includes explicit 'Trigger when' conditions to prevent hallucination, defines a clear configuration priority hierarchy, and provides extensive CLI flag documentation optimized for terminal-based agents.

**Summary:** Provides a comprehensive agent skill for document parsing using the GLM-OCR SDK via Python and CLI.

**Source credibility:** Highly credible source with nearly 7k stars on the underlying repository.

**Recency:** Very current; follows modern agentic patterns for environment management and CLI interaction.

**Source:** [zai-org/GLM-OCR/skills/sdk/SKILL.md](https://github.com/zai-org/GLM-OCR/blob/cef4d0ea120d1741f5cefe8985eee45f6c8eff1d/skills/sdk/SKILL.md) · 6963★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: glmocr
description: |
  Trigger when: (1) User wants to extract text, tables, formulas, or structured data from images/PDFs/scanned documents, (2) User mentions "OCR", "文字识别", "文档解析", (3) User has a document (screenshot, scanned page, invoice, paper, whiteboard photo) and needs its content in structured form, (4) User asks to parse, digitize, or extract content from a visual document.

  Invokes the GLM-OCR SDK (pip install glmocr) to parse documents via Zhipu's cloud API. No GPU required. Returns structured JSON (regions with labels + bounding boxes) and Markdown. Agent can operate entirely via CLI — no YAML files needed.

  NOT for: real-time camera feeds, audio transcription, or non-document images (photos, illustrations).
metadata:
  openclaw:
    requires:
      env:
        - ZHIPU_API_KEY
      bins:
        - python
    primaryEnv: ZHIPU_API_KEY
    emoji: "📄"
    homepage: https://github.com/zai-org/GLM-OCR/tree/main/skills/sdk
---

# OpenClaw Skill: glmocr

Parses documents (images, PDFs, scans) via the GLM-OCR SDK.

> **📌 On-demand**: This skill requires only `ZHIPU_API_KEY` in the environment. No YAML config files or GPU needed.

## ⚡ Quick Start

```bash
# In
```

</details>
