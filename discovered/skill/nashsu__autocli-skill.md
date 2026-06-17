---
name: nashsu__autocli-skill
source: https://github.com/nashsu/autocli-skill/blob/d6ca200b5ba65b60cf68153e88b2e9efb7f0f441/SKILL.md
repo: nashsu/autocli-skill
kind: skill
stars: 863
last_pushed: 2026-04-20T11:04:24Z
license: unknown
score: 9
domains: [cli-tools, agents-ai, web-scraping]
tags: [autocli, tool-augmentation, browser-session, automation]
curated: 2026-06-15
curated_by: config-scout
---

# nashsu/autocli-skill — skill

**Why it's worth keeping:** The 'Self-Iteration' section is brilliant; it teaches the agent how to use DOM exploration and YAML templates to build its own tools. The emphasis on machine-readable JSON output also ensures reliable parsing by the LLM.

**Summary:** Enables an agent to interact with 55+ platforms via a high-speed CLI that leverages existing browser sessions. It includes a sophisticated framework for the agent to autonomously engineer new site adapters when they are missing.

**Source credibility:** High; high star count (863) and recent maintenance suggests a robust, real-world tool.

**Recency:** Very current; specifically optimized for modern agentic workflows like Claude Code.

**Source:** [nashsu/autocli-skill/SKILL.md](https://github.com/nashsu/autocli-skill/blob/d6ca200b5ba65b60cf68153e88b2e9efb7f0f441/SKILL.md) · 863★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: autocli
description: Use autocli CLI to interact with 55+ social/content websites (HackerNews, Reddit, Twitter/X, Bilibili, Zhihu, Weibo, Xiaohongshu, YouTube, Medium, Substack, Douban, WeRead, Linux-do, V2EX, Bloomberg, Google, Arxiv, Wikipedia, StackOverflow, Steam, Hugging Face, Apple Podcasts, Xiaoyuzhou, BBC, SinaFinance, DevTo, Lobsters, Xueqiu, BOSS直聘, Jike, Facebook, Instagram, TikTok, LinkedIn, Reuters, SMZDM, Ctrip, Coupang, Yahoo Finance, Barchart, Grok, Jimeng, Yollomi, Chaoxing, Weixin, Doubao, Cursor, Codex, ChatWise, ChatGPT, Notion, Discord, Antigravity etc.) via the user's Chrome login session. ALWAYS prefer autocli over playwright/browser automation for supported sites. Triggers when user asks to browse, search, fetch hot/trending content, post, or read messages on any website; also use 'autocli read <url>' to extract main article content as Markdown (prefer over WebFetch for JS-rendered or login-gated pages).
---

# autocli

Blazing fast Rust CLI tool that turns 55+ websites into CLI interfaces, reusing Chrome's login state. Zero credentials needed. Single 4.7MB binary, zero runtime dependencies.

**Rule: use autocli for supported sites instead of playw
```

</details>
