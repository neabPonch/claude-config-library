---
name: skyllwt__AutoSci__skill
source: https://github.com/skyllwt/AutoSci/blob/71469e89eb1381e557661da0b90c0585c48288d7/i18n/zh/skills/poster/SKILL.md
repo: skyllwt/AutoSci
kind: skill
stars: 1250
last_pushed: 2026-06-14T10:13:48Z
license: mit
score: 9
domains: [academic-research, cli-tools, latex-automation]
tags: [poster-generation, content-distillation, html-rendering]
curated: 2026-06-15
curated_by: config-scout
---

# skyllwt/AutoSci — skill

**Why it's worth keeping:** Demonstrates excellent use of an intermediate representation (dag.json) and intelligent state persistence (caching author data in .txt files) to minimize redundant user interaction.

**Summary:** Converts LaTeX research papers into self-contained HTML academic posters using a sophisticated multi-step distillation and rendering pipeline.

**Source credibility:** High; part of the highly-starred AutoSci project which aims for a full-lifecycle AI research platform.

**Recency:** Current; utilizes advanced Claude Code capabilities like structured interactive questions and tool-based file manipulation.

**Source:** [skyllwt/AutoSci/i18n/zh/skills/poster/SKILL.md](https://github.com/skyllwt/AutoSci/blob/71469e89eb1381e557661da0b90c0585c48288d7/i18n/zh/skills/poster/SKILL.md) · 1250★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
description: 从已撰写的论文生成学术海报 —— 提炼章节为单页 HTML 海报,包含配图和段落间过渡
argument-hint: "[paper-dir] [--review] [--anonymous] [--no-figures] [--no-logos] [--no-refine]"
---

# /poster

> 从已撰写的论文生成学术 HTML 海报。读取 `paper/main.tex`、章节文件与图片;
> 构建 PaperX 兼容的 `dag.json` 中间格式;将每个章节提炼为 2–5 句话摘要;
> 选取代表性配图;渲染为自包含的 HTML 海报(三栏自适应布局)。

## Inputs

### 常用

- `paper_dir`(可选,默认 `paper/`):LaTeX 项目目录,需包含 `main.tex` 和 `sections/`
- `--review`(可选):调用 Review LLM 对生成的海报内容进行跨模型评审
- `--anonymous`(可选):强制将作者写为 "Anonymous",忽略 `\author{}`、`paper/.author_display.txt` 缓存以及 `--authors` flag
- `--no-figures`(可选):所有章节渲染为纯文本(适合文本密集型海报,或配图尚未准备好时)
- `--no-logos`(可选):跳过 affiliation / conference logo 询问,header 只显示 venue 文本
- `--no-refine`(可选):跳过 Step 5.5 critique-revise(默认会跑 1 轮)

### 进阶(脚本化使用;交互场景一般用不到)

- `--authors STR`:覆盖海报上的作者文本(例如 `--authors "Mingtian Yang, Co-Author"`)。一次性覆盖用;日常需求由 Step 0 Q1 的 `paper/.author_display.txt` 缓存自动处理。`--anonymous` 同时传入时仍以 `--anonymous` 为准。
- `--venue STR`:header 右块的 venue 文本(例如 `"NeurIPS 2026"`)。跳过 Step 0 的 venue 询问。
- `--affiliation-logo PATH` / `--conference-logo PATH`:logo 文件路径(PNG/JPG/PDF);各自跳过 Step 0 对应的询问。
- `--layout corners|stacked`(默认 `corners`):header 布局。`corners` = 单位 logo 左上 + 会议 logo 右
```

</details>
