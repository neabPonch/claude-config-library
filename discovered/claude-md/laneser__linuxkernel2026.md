---
name: laneser__linuxkernel2026
source: https://github.com/laneser/linuxkernel2026/blob/074d72c7873678a6a280787d75ed109d5fb5aea5/CLAUDE.md
repo: laneser/linuxkernel2026
kind: claude-md
stars: 0
last_pushed: 2026-04-18T04:50:08Z
license: unknown
score: 9
domains: [education, systems-programming, linux-kernel, knowledge-management]
tags: [learning-pathway, interaction-logging, documentation-standards, system-architecture]
curated: 2026-06-15
curated_by: config-scout
---

# laneser/linuxkernel2026 — claude-md

**Why it's worth keeping:** Includes a brilliant 'Interaction Process' pattern to document human-AI collaboration and a strategic 'Progressive Disclosure' logic for how Claude should fetch/process reference materials.

**Summary:** A highly sophisticated orchestration file for an AI-assisted learning environment that manages complex documentation and knowledge-tracking workflows.

**Source credibility:** High-quality personal educational project with extremely structured, professional documentation standards.

**Recency:** Very current; uses advanced agentic patterns like specific tool-use instructions (curl vs WebFetch).

**Source:** [laneser/linuxkernel2026/CLAUDE.md](https://github.com/laneser/linuxkernel2026/blob/074d72c7873678a6a280787d75ed109d5fb5aea5/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — 專案指引

本文件供 Claude CLI 讀取，作為與使用者協同工作時的上下文基礎。

## 專案概述

本專案是一個以 AI 驅動的 Linux Kernel 學習環境，目的是讓學習者與 Claude 協同學習 Linux Kernel 2026 課程。Claude 在本專案中身兼 **助手** 與 **老師**，協助閱讀原始碼、解釋概念，並從中提供洞見以加速學習。

## 架構文件

本專案採用 **ARC42** 作為架構文件模板，位於：

- [`docs/ARC42.md`](docs/ARC42.md) — 完整架構文件

在回答架構相關問題時，請優先參考 ARC42 文件。

## 參考文件

`docs/references/` 目錄存放課程相關的參考資料（論文、規格書、教材摘要等），目的是讓 Claude 能快速取用，減少重複說明的溝通成本。

回答問題時，若 `docs/references/` 中有相關資料，請優先引用。

### 漸進式揭露原則

參考文件採用 **漸進式揭露（Progressive Disclosure）** 策略，根據來源品質決定本地存放深度：

| 來源狀況 | 本地存放 | Claude 行為 |
|----------|---------|------------|
| **課程教材**（`hackmd.io/@sysprog/` 開頭） | **完整 raw markdown** | 用 `curl` 抓 `/download` 端點，直接讀取本地檔案（見下方說明） |
| **其他結構良好的來源** | 摘要 + metadata | 需要細節時從原始出處 `WebFetch` 抓取 |
| **結構不佳**（PDF、無分段長頁面等） | 本地存完整整理版 | 直接讀取本地檔案 |

每個參考檔案的 header 包含以下 metadata：

```markdown
> **原始出處：** URL（Claude 按需取用的來源）
> **擷取日期：** YYYY-MM-DD
> **用途：** 說明
> **涵蓋度：** 完整 / 摘要（約 N%）
> **省略內容：** 被省略的主要段落（僅摘要版填寫）
```

#### 參考文件索引

| 檔案 | 用途 |
|------|------|
| `n1256-c99.md` | ISO/IEC 9899:TC3 (C99) 規格書完整 markdown 轉換 |
| `it-vocabulary.md` | 資訊科技詞彙翻譯 |
| `warmup.md` | 第一週作業 (warmup) 完整要求 |
| `ai-guidelines.md` | 本課程 AI 工具使用規範 |
| `linux-course-sch
```

</details>
