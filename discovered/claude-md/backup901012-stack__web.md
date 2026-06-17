---
name: backup901012-stack__web
source: https://github.com/backup901012-stack/web/blob/f77bc3017a77fc5f4a52fe210433df57410f23ae/CLAUDE.md
repo: backup901012-stack/web
kind: claude-md
stars: 0
last_pushed: 2026-04-17T11:04:45Z
license: unknown
score: 9
domains: [web-frontend, fullstack, ai-integration]
tags: [qa-checklist, defensive-coding, impact-assessment]
curated: 2026-06-15
curated_by: config-scout
---

# backup901012-stack/web — claude-md

**Why it's worth keeping:** The 'Self-Correction Mechanism' forces the agent to perform impact assessment and cross-dependency checks (e.g., Prompt ↔ Frontend ↔ PDF) before writing code. The specific QA table provides an actionable framework for verifying complex business logic transitions.

**Summary:** Implements a rigorous three-layer self-correction mechanism and a mandatory QA checklist to manage high-stakes full-stack dependencies.

**Source credibility:** High-detail personal project with a very active, high-frequency development history showing complex bug resolutions.

**Recency:** Extremely current, targeting modern Next.js 14 and AI integration workflows.

**Source:** [backup901012-stack/web/CLAUDE.md](https://github.com/backup901012-stack/web/blob/f77bc3017a77fc5f4a52fe210433df57410f23ae/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# 鑑源網頁製作

## 專案簡介
鑑源命理平台（jianyuan.life）前端網頁開發專案。
Next.js 14 App Router + Tailwind CSS + Supabase + Stripe + Vercel 部署。

**網站版本：** v4.5.24（2026-04-11）
**線上網址：** https://jianyuan.life
**Vercel 專案：** fortune-reports（對應 backup901012-stack/qimen-chumenji）

## 溝通語言
- 一律使用**繁體中文**溝通、討論、說明

## 自我糾錯機制（強制性，不可跳過）

### 第一層：改動前 — 影響評估（必做）
每次改程式碼前，必須先回答三個問題：
1. **影響範圍**：這個改動影響哪些頁面/功能？列出所有受影響的檔案
2. **最壞情況**：1000 人同時用會發生什麼？會不會破產？
3. **連動檢查**：有沒有其他地方用到同一段邏輯需要同步改？
   - 改 Prompt → 必須同步改品質閘門 regex + 前端渲染
   - 改前端格式 → 必須同步改 PDF 渲染 + Email 模板
   - 改 API → 必須同步改 fallback 路徑
   - 改方案內容 → 必須同步改定價表 + 結帳頁 + FAQ

### 第二層：改動中 — 即時檢查（必做）
- 每個檔案改完立刻跑 `npm run type-check`，不等全部改完
- 改了 A 就搜尋所有引用 A 的地方，確認不會壞 B

### 第三層：推送前 — QA Agent 強制稽查（不可跳過）
**任何改動，不管大小，推送前必須開 QA Agent 做八大項稽查：**

| # | 稽查項 | 怎麼查 | 不過就不推 |
|:---:|:---|:---|:---:|
| 1 | TypeScript 零錯誤 | `npm run type-check` | ✅ |
| 2 | Build 成功 | `npm run build` | ✅ |
| 3 | 改動不影響其他功能 | 搜尋所有引用同一函式/變數的地方 | ✅ |
| 4 | 前後端一致 | Prompt ↔ 品質閘門 ↔ 前端渲染 ↔ PDF ↔ Email | ✅ |
| 5 | 文案不過度承諾 | 定價表/結帳/FAQ 跟實際報告對齊 | ✅ |
| 6 | 安全性 | API 權限、RLS、input validation | ✅ |
| 7 | 1000 人壓力思考 | 併發/超時/rate limit 有沒有受影響 | ✅ |
| 8 | 回歸測試 | 確認修 A 沒壞 B | ✅ |

**八項全過才能 git push。任何一項失敗就停下來修，修完重新跑 QA。
```

</details>
