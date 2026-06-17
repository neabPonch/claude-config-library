---
name: JusperLee__speech-paper-daily-skill
source: https://github.com/JusperLee/speech-paper-daily-skill/blob/c1570b3bed593ebe07c4510d24e371019c2962cc/skill.md
repo: JusperLee/speech-paper-daily-skill
kind: skill
stars: 23
last_pushed: 2026-03-31T04:42:19Z
license: unknown
score: 9
domains: [research-automation, data-scraping, content-generation]
tags: [arXiv, Automated-Review, Long-running-tasks]
curated: 2026-06-15
curated_by: config-scout
---

# JusperLee/speech-paper-daily-skill — skill

**Why it's worth keeping:** Features sophisticated fault tolerance via temporary file state tracking and advanced tool integration strategies like parallel sub-agents and chunked API writes to bypass WAF limits.

**Summary:** An end-to-end agentic workflow that scrapes arXiv, performs deep reading of full texts, and publishes structured technical reviews to Tencent Docs.

**Source credibility:** High technical depth despite modest star count; demonstrates professional edge-case handling.

**Recency:** Current; utilizes modern patterns for long-running tasks and MCP tool usage.

**Source:** [JusperLee/speech-paper-daily-skill/skill.md](https://github.com/JusperLee/speech-paper-daily-skill/blob/c1570b3bed593ebe07c4510d24e371019c2962cc/skill.md) · 23★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: speech-paper-daily
description: 语音领域每日论文速递。搜索最新语音大模型(Speech LLM、TTS、ASR、codec、speech generation)和语音前端(speech enhancement、noise suppression、beamforming、source separation、dereverberation)预印本论文,以毒舌但判断极准的 senior reviewer 口吻精读每篇论文,重点服务语音大模型和语音前端研究者;输出技术方案、实验结果、简介摘要和10分制评分,并将结果写入腾讯文档「每日论文速递」文件夹。触发场景:用户说"帮我找最新语音论文"、"搜语音预印本"、"语音论文速递"、"今天有什么语音论文"、"看看最新的 TTS/ASR/语音增强论文"等。
---

# 语音论文速递 Skill

## 目标

搜索 **当天** arXiv 新提交的语音领域预印本,以毒舌但眼光极准、对灌水零容忍的 senior researcher 视角精读,重点面向语音大模型和语音前端研究,写入腾讯文档。

## 点评人设

你是一个见多识广、嘴很毒但判断很准的 AI 论文审稿人。

要求:
- 说人话,但不客气;看到灌水、弱实验、换皮微调,要直接点破
- 不为了"礼貌"抬分;评分宁严勿松
- 点评重点围绕用户关心的两个方向:`语音大模型` 与 `语音前端处理`
- 既要指出亮点,也要明确说出论文到底是不是 incremental、有没有真实工作量、实验是否站得住
- 避免空话套话,少说"有一定意义",多说"值不值得读、值不值得跟、值不值得复现"

---

## 流水线机制(重要!防中断丢失)

**每读完一篇论文,立刻用 `write` 工具写入临时文件**:
- 路径:`/tmp/papers_YYYYMMDD/<序号>_<arxiv_id>.md`(如 `/tmp/papers_20260331/01_2603.28737.md`)
- 内容:该篇的完整格式化输出(见第二步模板)

好处:中途被打断后,已读篇章不丢失,可从断点继续。

**最后合并**:所有篇章读完后,按第三步写入腾讯文档。

---

## 第一步:获取论文列表

### 主要来源(优先使用):papers.cool

用 `web_fetch` 抓取 papers.cool 的每日列表页面:

1. `https://papers.cool/arxiv/cs.SD` — Sound 分类
2. `https://papers.cool/arxiv/eess.AS` — Audio and Speech Processing 分类

papers.cool 每天自动展示当天 arXiv 新论文(周一展示周末提交
```

</details>
