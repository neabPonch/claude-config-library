---
name: little-jax__bilibili-all-in-one
source: https://github.com/little-jax/bilibili-all-in-one/blob/2c3daa08bd0a725ba5ee53bd63d59a61ab592e5e/skill.md
repo: little-jax/bilibili-all-in-one
kind: skill
stars: 1
last_pushed: 2026-04-08T11:32:20Z
license: mit-0
score: 9
domains: [cli-tools, automation, social-media]
tags: [workflow-heavy, domain-specific]
curated: 2026-06-14
curated_by: config-scout
---

# little-jax/bilibili-all-in-one — skill

**Why it's worth keeping:** It utilizes advanced agentic patterns like 'operating instincts' to handle user ambiguity and a 'reading map' to optimize context window efficiency by directing the LLM to specific reference files.

**Summary:** A highly specialized toolkit for Bilibili creator operations including live stream orchestration, community management, and content publishing via CLI.

**Source credibility:** Niche/specialized repository with recent activity.

**Recency:** Very current (2 months ago) and perfectly aligned with modern tool-use/agentic reasoning paradigms.

**Source:** [little-jax/bilibili-all-in-one/skill.md](https://github.com/little-jax/bilibili-all-in-one/blob/2c3daa08bd0a725ba5ee53bd63d59a61ab592e5e/skill.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: bilibili-all-in-one
description: >
  A Bilibili creator-operations toolkit for creator/community workflows:
  live start/stop/recovery/runtime sampling, dynamic posting/repost/delete,
  comment/reply handling, message/reply triage, follower/community ops, plus
  download/watch/subtitle/publishing support. Use when the user talks about
  开播, 下播, 继续上次直播, 直播间标题/分区/公告, 发动态, 回动态, 回评论,
  处理B站回复/消息, or general Bilibili creator operations with authenticated cookies.
version: 1.0.18
type: code
implementation: python
interface: cli-and-api
runtime: python>=3.8
languages:
  - zh-CN
  - en
tags:
  - bilibili
  - video-download
  - hot-trending
  - subtitle
  - danmaku
  - video-publish
  - video-player

  - batch-download
  - multi-format
author: Little Jax / Mozi A.
license: MIT-0
homepage: https://github.com/little-jax/bilibili-all-in-one
repository: https://github.com/little-jax/bilibili-all-in-one
original_author: wscats
upstream_repository: https://github.com/wscats/bilibili-all-in-one
entry_point: main.py
required_env_vars: []
optional_env_vars:
  - BILIBILI_SESSDATA
  - BILIBILI_BILI_JCT
  - BILIBILI_BUVID3
  - BILIBILI_PERSIST
install: pip install -r requirements.txt
---

##
```

</details>
