---
name: tiankonguse__evo-agent__06-skill
source: https://github.com/tiankonguse/evo-agent/blob/003fb316078353713376cf86a8e18d50c5c2f615/blog/06-skill.md
repo: tiankonguse/evo-agent
kind: skill
stars: 5
last_pushed: 2026-06-10T12:56:04Z
license: unknown
score: 9
domains: [agents-ai, workflow-automation]
tags: [skill-system, lazy-loading, prompt-engineering, agentic-workflows]
curated: 2026-06-15
curated_by: config-scout
---

# tiankonguse/evo-agent — skill

**Why it's worth keeping:** Solves context window bloat through lazy-loading; provides a highly structured template (YAML manifest + Markdown steps) for turning complex business logic into repeatable agent actions.

**Summary:** Implements an 'On-Demand Skill' architecture that uses a lightweight catalog of descriptions to trigger loading full task workflows only when necessary.

**Source credibility:** 5 stars on GitHub, very active development as of the source date.

**Recency:** Highly current approach to solving LLM context/token efficiency challenges.

**Source:** [tiankonguse/evo-agent/blog/06-skill.md](https://github.com/tiankonguse/evo-agent/blob/003fb316078353713376cf86a8e18d50c5c2f615/blog/06-skill.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
layout: post
title: 聊聊 Agent Skill：把经验变成可复用的工作流
description: Agent 能调工具了，但复杂任务总要从头靠 LLM 自己摸索。这篇聊聊 Skill 的设计思路，再看 evo-agent 如何实现一个轻量的 Skill 系统，最终用一个字段溯源 Skill 替换掉一个 hardcode 的专用 Agent。
keywords: 项目实践
tags: [agent, skill, workflow, golang]
categories: [程序人生]
updateDate: 2026-05-15 12:00:00
published: true
source: "https://mp.weixin.qq.com/s/X2ie0aQ2vMtddAQrkbOG5g"
---

![截图](https://res2026.tiankonguse.com/images/2026/05/15/003.png)


前五篇文章分别讲了 Agent 的 [Loop](https://mp.weixin.qq.com/s/dkdrwVlwe3IkH2hzSzy53A)、[Tools](https://mp.weixin.qq.com/s/xyX4_CF5cveezEDuzFT13g)、[记忆](https://mp.weixin.qq.com/s/lguRAdxFoN22rqPyx3BIzw)、[Context Compact](https://mp.weixin.qq.com/s/YRS29wRckEmFgNb0eJrxrQ) 和 [MCP](https://mp.weixin.qq.com/s/rCnGif8Ee7JhRI86-RoNWA)。  


这篇聊一个更贴近实用的话题——Skill。  


先说一个你大概率遇到过的问题。  


Agent 有了工具，有了 MCP，能干的事越来越多了。  
但你会发现一个很别扭的事：每次遇到复杂任务，LLM 都在从零开始摸索。  
该调哪些工具、按什么顺序、中间结果怎么处理，它得自己想。  


这就好比你公司来了个新人，聪明是真聪明，但每次接活都得自己重新摸索一遍流程。  
明明上次已经跑通了，这次又从头来。  


有没有办法把这套"经验"固化下来，让它下次直接复用？  


这就是 **Skill** 要解决的问题。  


## 先说说痛在哪里

说个我自己在项目里踩过的坑。  


我们内部有一个数据服务叫 UnionPlus，存着海量媒体内容的各种字段。  
字段的值来源很复杂——有的直接存在 Redis 里，有的要通过计算表达式从依赖字段推导，有的还得查枚举翻译表才能拿到最终的可读值。  


当时怎么做的呢？  
写了一个**专用 Agent*
```

</details>
