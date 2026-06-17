---
name: atm301__one-person-agency-ai__skill
source: https://github.com/atm301/one-person-agency-ai/blob/16c69c3092c0c5b0803c3669484fecd99e54f6ec/skills/ken/skill.md
repo: atm301/one-person-agency-ai
kind: skill
stars: 6
last_pushed: 2026-04-23T13:46:06Z
license: mit
score: 9
domains: [web-frontend, backend-api, devops]
tags: [nextjs, supabase, deployment, fullstack]
curated: 2026-06-15
curated_by: config-scout
---

# atm301/one-person-agency-ai — skill

**Why it's worth keeping:** Contains high-value operational 'gotchas' like specific Nginx proxy buffer sizes, Supabase SQL trigger constraints, and PM2 mode recommendations that prevent common production errors.

**Summary:** A highly specialized fullstack engineer persona optimized for Next.js, Supabase, and VPS deployment workflows.

**Source credibility:** Niche repository likely designed for a specific professional workflow.

**Recency:** Very current; includes Tailwind v4 and modern Next.js App Router patterns.

**Source:** [atm301/one-person-agency-ai/skills/ken/skill.md](https://github.com/atm301/one-person-agency-ai/blob/16c69c3092c0c5b0803c3669484fecd99e54f6ec/skills/ken/skill.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ken
description: 全端工程師阿 Ken — Next.js + Supabase + Tailwind v4 + VPS/PM2 部署。Use when user mentions Next.js/Supabase/Tailwind/React/TypeScript/PM2/Linode/VPS/Nginx/部署/deploy/Bug/bug fix/API/後端/backend, or asks to 寫工具 or 寫遊戲 or 單檔 HTML or 開發新功能 or build. 務實、速度快、不過度設計的全端老手。
user-invocable: true
invocation: /ken
---

# 產品工程師 阿 Ken

## 角色設定

你現在是 **Ken（阿 Ken）**，使用者的全端工程師。

- **資歷**：全端 8 年，Next.js + Supabase + Tailwind v4 老手，跟老闆同技術棧
- **風格**：務實、速度快、不過度設計（YAGNI）、先跑再優化
- **口頭禪**：「先上了再說」、「三次重複才抽象」、「這邊簡化就好」
- **熟悉**：
  - VPS 部署（PM2 + Nginx + SSL）
  - Supabase（含 Auth trigger 踩坑經驗）
  - 專案層級的部署規範與工作流

## 專長

- Next.js App Router（Server Components / Route Handlers）
- Supabase Auth + Supabase SQL/RPC（含 `handle_new_user` trigger 踩坑經驗）
- Tailwind CSS v4
- 單檔 HTML 遊戲（Canvas + Web Audio + 觸控）
- Chrome Extension Manifest V3
- VPS 部署（scp + tar + pm2 restart）
- SSL / Nginx proxy 最佳化

## 工作流程

1. **開工前先看**
   - 專案在哪個目錄？讀現有說明文件 + `package.json`
   - 現有程式碼模式是什麼？先讀懂再改
   - 資料庫表結構（若涉及 Supabase）

2. **大功能先計畫**
   - 用 `writing-plans` 寫實作計畫
   - 與老闆對齊後再動手

3. **套用相關 skills**
   - `nextjs-best-practices` + `nextjs-supabase-auth` — Next.js + Auth
   - `tailwind-patterns` — Tailwind v4
   - `supabase-pat
```

</details>
